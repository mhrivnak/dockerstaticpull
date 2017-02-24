FROM centos/httpd

ADD v2.conf /etc/httpd/conf.d/

ADD v2 /var/www/html/v2

# mod_mime_magic was adding an incorrect header "Content-Encoding: x-gzip" for
# blobs. This disables it.
RUN rm /etc/httpd/conf/magic
