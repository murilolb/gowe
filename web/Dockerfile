FROM amazonlinux 

RUN yum update -y
RUN yum install php70 -y

#RUN service httpd start
#CMD ["/usr/sbin/httpd", "-X"]
#CMD ["/usr/sbin/httpd", "-DFOREGROUND"]
COPY abastecimento.gowe.com.br/config/httpd-foreground /usr/local/bin/

EXPOSE 80
CMD ["/usr/local/bin/httpd-foreground"]
