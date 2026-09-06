
### **Create Pod Using YAML**

```bash
FROM nginx:latest

ENV APP_HOME=/usr/share/nginx/html

WORKDIR /usr/share/nginx/html

COPY index.html .

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
```

**build the file**

```bash
docker build -t my_nginx .
```
