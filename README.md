# HelloWorld
Homework Assignment #1 Hello World API


## Prerequisite Requirements

* It should be a RESTful JSON API that listens on a port of your choice
* When someone posts anything to the route /hello, you should return a welcome message, in JSON format. This message can be anything you want.


## Local Development/Testing

**IMPORTANT NOTE:** Unless you have your SSL certs in created directory `https` on the root level. It won't create an HTTPS Server

1. [Fork](https://help.github.com/articles/fork-a-repo/) this repository.
2. On your local machine. `cd` into `HelloWorld`
3. For `staging` environment, run the command below and verify the port in the logs

```sh
$> node index.js
The HTTP server is running on port 3000
The HTTPS server is running on port 3001
```

4. For `production` environment, run the command below and verify the port in the logs
```sh
$> NODE_ENV=production node index.js
The HTTP server is running on port 5000
The HTTPS server is running on port 5001
```


## Verify API sanity

1. Jump to your application for testing REST APIs
2. POST/GET requests to `localhost:3000/hello`
3. Verify the following output
```json
{
  "message": "Welcome onboard"
}
```