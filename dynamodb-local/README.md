# How to use this image

### start a dynamodb instance

```
docker run -it --name test-dynamo fitz/dynamodb-local
```

This image includes `EXPOSE 8000` (the dynamodb local port), so standard container linking will make it automatically available to the linked containers (as the following examples illustrate).


### connect to it from an application

```
docker run --name some-app --link test-dynamo:dynamodb -d application-that-uses-dynamodb
```


### start an in memory dynamodb instance

```
docker run -it fitz/dynamodb-local -inMemory
```
