FROM nginx:1.21.6-alpine-perl

WORKDIR /usr/share/nginx/html
COPY /html/. /usr/share/nginx/html/

RUN apk update
RUN apk add bash
RUN apk add git

EXPOSE 80
STOPSIGNAL SIGQUIT

CMD ["nginx", "-g", "daemon off;"]
