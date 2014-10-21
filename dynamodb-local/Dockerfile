FROM dockerfile/java:oracle-java8

MAINTAINER Ryan Fitzgerald, ryan.fitz1@gmail.com

RUN /usr/bin/curl -L http://dynamodb-local.s3-website-us-west-2.amazonaws.com/dynamodb_local_latest.tar.gz | /bin/tar xz

WORKDIR /data

ENTRYPOINT ["/usr/bin/java", "-Djava.library.path=./DynamoDBLocal_lib", "-jar", "DynamoDBLocal.jar"]

CMD ["-help"]

EXPOSE 8000
