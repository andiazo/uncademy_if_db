# UNCADEMY FINANCIAL INFORMATION DATABASE

Configuration to mount the database in postgresql necessary for the financial information microservice.

On Dockerfile set your own values for the variables, 

```Dockerfile
ENV POSTGRES_ROOT_PASSWORD=<YOUR_ROOT_PASSWORD>
ENV POSTGRES_DB=<YOUR_DB_NAME>
ENV POSTGRES_USER=<YOUR_DB_USER>
ENV POSTGRES_PASSWORD=<YOUR_DB_PASSWORD>
```

then run:

```cmd
docker build -t uncademy_if_db .
docker run -d -t -i -p 5432:5432 --name uncademy_if_db uncademy_if_db
```
