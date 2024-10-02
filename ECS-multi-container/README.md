## This is the application structure

```md
├── app.py
├── docker-compose.yml
├── Dockerfile
├── README.md
└── requirements.txt
``` 

## Multi Docker run with command 

```md
docker run --name my-postgres -e POSTGRES_USER=myuser -e POSTGRES_PASSWORD=mypassword -e POSTGRES_DB=mydb -p 5432:5432 -d postgres

docker build -t my-python-app .

docker run -dit --link my-postgres:db --name my-python-app  -p 8001:8000 my-python-app
```

# Important to know

**Make sure to change db host ip address in app.py and build the python app after you successfully deployed db container in ECS**
