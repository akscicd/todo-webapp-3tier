FROM nginx:stable-perl
RUN rm -rf /usr/share/nginx/html/*
COPY build /usr/share/nginx/html/
#WORKDIR /usr/share/nginx/html/
#RUN cp -rf build/* .
RUN rm -rf /etc/nginx/conf.d/default.conf
COPY default.conf /etc/nginx/conf.d/default.conf
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
