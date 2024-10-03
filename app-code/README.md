## Steps to run on your local

**Make sure to install nodejs and npm packages**

`
    npm init -y
`
    
    npm install express
    node index.js


## Steps to run with docker
`
    docker build -t mynodjsapp .
`

    docker run -d --name nodejscontainer -p 3000:3000 mynodejsapp:latest

    docker push mrnanda/mynodjsapp:v1.0