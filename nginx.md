FROM nginx:latest

ENV APP_HOME=/usr/share/nginx/html/

WORKDIR usr/share/nginx/html

COPY index.html /usr/share/nginx/html/

RUN apt-get update -y

EXPOSE 80 

CMD ["nginx","-g","daemon off;"]

  

