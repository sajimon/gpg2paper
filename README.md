# gpg2paper
Generate PDF document with secret GPG keys or revocation certificates using pdflatex.

Credits goes to @costrouc.

Example usage:

```bash
pdflatex -shell-escape "\\def\gptitle{Master Key}\\def\gpkeyfinger{478122ED}\\def\gpfile{data.bin}\\include{gpg2paper}"
```

The *data.bin* file contains your secret data or any other data you wish to backup. It can contain the output of
```
gpg --output data.bin --export-secret-key [YOURKEYID]
```
but it's recommended to use [paperkey](http://www.jabberwocky.com/software/paperkey/) utility to extract only secret data. It will produce less bytes to backup and make QR codes less dense.

Remember to destory your printer afterwards, preferably with :fire:!

Example output:

![alt tag](https://user-images.githubusercontent.com/402648/40799965-57824dca-650f-11e8-94e4-e9e4a2c0c5fa.png)
