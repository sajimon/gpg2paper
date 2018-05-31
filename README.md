# gpg2paper
Generate PDF document with secret GPG keys or revocation certificates using pdflatex.

Credits goes to @costrouc.

Example usage:

```bash
pdflatex -shell-escape "\\def\gptitle{Master Key}\\def\gpfile{key.bin}\\include{gpg2paper}"
```
![alt tag](https://user-images.githubusercontent.com/402648/40799965-57824dca-650f-11e8-94e4-e9e4a2c0c5fa.png)
