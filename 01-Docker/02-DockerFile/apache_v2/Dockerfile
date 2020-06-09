# Base Image
FROM ubuntu:16.04

# Owner 
MAINTAINER Amit Vashist

# Update Apt Repo
RUN apt-get update

# Install Apache Packages
RUN apt-get install apache2 -y 

# Copy Custom Web Page
COPY info.html /var/www/html/

# My Service Linten on Port
EXPOSE 80 
EXPOSE 3306 

# Bring up the Service
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
