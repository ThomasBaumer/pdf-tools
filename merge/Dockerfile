FROM ubuntu:16.04
RUN apt update; apt install pdftk ghostscript -y
WORKDIR /tmp
RUN echo "#!/bin/bash\npdftk /tmp/*.pdf cat output /tmp/merged.pdf\ngs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/screen -dNOPAUSE -dQUIET -dBATCH -sOutputFile=/tmp/compressed.pdf /tmp/merged.pdf" > /opt/entrypoint.sh; chmod u+x /opt/entrypoint.sh 
CMD ["/opt/entrypoint.sh"]