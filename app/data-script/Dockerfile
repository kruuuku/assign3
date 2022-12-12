FROM alpine:latest
RUN apk update
RUN apk add mysql-client
WORKDIR /opt
COPY import.sh .
COPY mydatabase.sql .
RUN chmod +x import.sh 
RUN chown root:root import.sh
CMD ./import.sh
