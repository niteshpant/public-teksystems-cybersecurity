FROM nginx:1.10.1-alpine # only downloading docker image from trusted image source (docker hub)
COPY index.html /usr/share/nginx/html
EXPOSE 8080 # only exposing the post what is required.
CMD ["nginx", "-g", "daemon off;"]