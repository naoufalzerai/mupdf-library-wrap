# mupdf-library-wrap
![example workflow](https://github.com/github/docs/actions/workflows/main.yml/badge.svg)
1. Download MuPDF code source: https://mupdf.com/releases/index.html 
2. Compile "usr/lib/libmupdf.so" : 
  `sudo make prefix=/usr shared=yes install`
3. Build library with 
  `go build -buildmode=c-shared -tags extlib -o pdf2jpeg.so`
