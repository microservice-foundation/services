

# Run microservices as a whole

Set environment variables for AWS:

```
export AWS_ACCESS_KEY_ID = your access key id
export AWS_SECRET_ACCESS_KEY = your secret access key
```

### Start microservices
```
docker-compose -f docker-compose.yaml up
```

### Examples
- Post a resource
```
curl --location --request POST 'http://localhost:8771/resources' \
--form 'multipartFile=@"/Users/Yusuf_Murodov/Downloads/mpthreetest.mp3"'
```

- Delete a resource
```
curl --location --request DELETE 'http://localhost:8771/resources?id=#saved_resouce_number'
```
