FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/daws-81s/expense-infra-dev/refs/heads/main/readme.MD /usr/share/nginx/html/index.html
RUN chmod +x /usr/share/nginx/html/index.html 
# RUN chmod -R 755 /usr/share/nginx/html/
# RUN chmod 644 /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]