FROM  ubuntu
WORKDIR /var/www/html 
#/var/www/html will be replaced by . now due to above line
RUN   apt update && apt install nginx -y
#above command is being merged with below command
#RUN   apt install nginx -y
#COPY index.html /var/www/html
ADD   index.html .
ADD   https://images.rawpixel.com/image_png_800/czNmcy1wcml2YXRlL3Jhd3BpeGVsX2ltYWdlcy93ZWJzaXRlX2NvbnRlbnQvcHUyMzMxNzg4LWltYWdlLXJtNTAzLTAxXzEtbDBqOXFyYzMucG5n.png dog.png
RUN   chmod 644 dog.png
CMD   nginx -g 'daemon off;'
