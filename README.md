# File upload system using JavaScript, Node.js, Express, MongoDB, Mongoose, Multer and Amazon S3

The system allows you to store uploaded files directly on the server with Multer or to store in the cloud using amazon s3. This setting can be done by changing the value of the 'STORAGE_TYPE' environment variable to 'local' or 's3'.

If you use Amazon S3, the environment variables 'AWS_ACCESS_KEY_ID', 'AWS_SECRET_ACCESS_KEY', 'AWS_S3_BUCKET_NAME' and 'AWS_DEFAULT_REGION' must be populated with the settings provided by Amazon.

For the database configuration, in development environment I suggest using Docker. Just run the following command:

```shell
docker run --name database -p 27017:27017 -d -t mongo
```

Replace database with the name you prefer.

The environment variable 'MONGO_URL' must be fed with the MongoDB connection url.
