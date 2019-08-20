# PdfUnlock
This script aims to remove modification restrictions from PDF files. 

The file must not be encrypted, and you must be able to **view** it.

## How it works
The script converts the input PDF file to PostScript files, and then back to PDF files. The resulting PDF files will be united again, creating the final PDF file.

## How to use
Call the script as follows:
```bash
pdfunlock [Locked PDF] [Unlocked PDF]
```

When the script has terminated, the unlocked PDF should be available at the destination path you provided.

## Installation
First make sure that you have the necessary tools installed. Normally one should install a standard TeXLive-Distribution, this includes all tools.
The following tools must be available in your PATH:
- ps2pdf
- pdftops
- pdfinfo
- pdfunite
- mktemp

When all prerequisites are installed, copy the script file to /usr/bin like this:
```bash
cp ./pdfunlock /usr/bin/pdfunlock
chmod +x /usr/bin/pdfunlock
```

## License
Copyright 2019 Stephan Brunner

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

