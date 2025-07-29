# Use the official Nginx image as a base
FROM ubuntu:latest

RUN apt-get update && apt-get install -y apache2

# Copy your web project files into the Nginx default web directory
COPY . /var/www/html
# Expose port 80 (Nginx default HTTP port)
EXPOSE 80

# Start Nginx when the container launches
CMD ["apache2ctl", "-D", "FOREGROUND"]