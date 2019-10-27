# pdf-tools
Add and compress multiple pdf files via Docker

## Requirements
- Docker

## Getting started 
- Execute for linux `../pdf-tools/merge/build.sh`
- Execute for windows `../pdf-tools/merge/build.bat`

## Run
- Execute `docker run -it -v /path/to/your/pdfs:/tmp/ pdf-tool-merge:latest` (you have to configure the path to your pdfs)
- There are two outputs:
  - /path/to/your/pdfs/merged.pdf: the merged pdf files
  - /path/to/your/pdfs/compressed.pdf: the compressed merged.pdf file
