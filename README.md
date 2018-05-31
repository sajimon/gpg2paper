# gpg2paper
Generate PDF document with secret GPG keys or revocation certificates using pdflatex.

Example usage:

```bash
pdflatex -shell-escape "\\def\gptitle{Master Key}\\def\gpfile{key.bin}\\include{gpg2paper}"
```
