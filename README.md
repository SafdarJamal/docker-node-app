# Dockerizing a Node.js web app

The goal of this example is to show you how to get a Node.js application into a Docker container.

## Development

To get a local copy of the code, clone it using git:

```
git clone https://github.com/SafdarJamal/docker-node-app.git
cd docker-node-app
```

Now that you have some source code and a Dockerfile, it’s time to build your first image:

```
docker build -t docker-node-app .
```

Start a container based on your new image:

```
docker run -d -p 8080:8080 docker-node-app
```

Visit your application in a browser at localhost:8080. You should see your hello world application up and running.

## License

This project is licensed under the terms of the [MIT license](https://github.com/SafdarJamal/docker-node-app/blob/master/LICENSE).
