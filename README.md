# Gatling Web Server
Fefe's Gatling HTTP Server as Docker Image, see https://www.fefe.de/gatling for details

## HTTP Server
`docker run -v /var/www:/var/www -p 80:80 -p 443:443 paulritter/gatling`

Keep in mind, that gatling will only serve world-readable files!

### Virtual Domains
See http://www.acme.com/software/thttpd/thttpd_man.html#MULTIHOMING for details.

You basically add subdirectories like `www.example.com` to your www-root.

## FTP
The images is started with the `-a` flag, that `chown`s all files you upload to make them downloadable again.

## SMB
to be documented
