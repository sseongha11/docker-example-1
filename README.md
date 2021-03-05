# Front End project

1. Building the docker

```sh
$docker build -f Dockerfile.dev .
```

Instead of the following commands

```sh
$docker build .
```

2. Run the docker container (or Starting the container)

Due to a recent update in the Create React App library, we will need to change how we start our containers.

In the upcoming lecture, you'll need to add the -it flag to run the container in interactive mode:

```sh
$docker run -it -p 3000:3000 IMAGE_ID
```

```sh
$docker run -it -p 3000:3000 -v /app/node
```

- **Final solution (Run the docker container)**

```sh
$docker-compose up
```

## Test

```sh
$docker build -f Dockerfile.dev .
```

And then, test

```sh
$docker run -it <Container ID> npm run test
```

## Make the internal instruction

```sh
$docker exec -it <Container ID> npm run test
```

## 2 tests (tests, web)

```sh
$docker-compose up --build
```

## docker attach (?)

```sh
$docker attach <container ID>
```

##

```sh
$docker exec -it <Container ID> sh
```

## Summary (Final docker build commands)

```sh
$docker build .
```

```sh
$docker run -p 8080:80 b0472726d87b
```

- 8080 means the port in the local laptop.
- 8080 means the port in the container

## Git setting

1. Git init

```sh
$git init
```

2. Git add

```sh
$git add .
```

3. commit

```sh
$git commit -m "initial commit"
```

```sh
$git remote add origin https://github.com/sseongha11/docker-react-1.git
```

```sh
$git push -u origin main
```
