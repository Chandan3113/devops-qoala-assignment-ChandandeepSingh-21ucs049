FROM nginx:latest

RUN rm /etc/nginx/conf.d/default.conf

# Copy our production-ready configuration
COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
