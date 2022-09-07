# Shop Microservices with .NET 6

### Steps to run the services

Update the connection strings in the `docker-compose.yml` file through the environment variables `CONNECTIONSTRINGS__DEFAULTCONNECTION`. In addition, update the images of the services to contain your registry of choice.

Navigate to the root of the folder and then build with docker-compose using the following command.
```bash
docker-compose build
```

After the build, you can then run `docker-compose up` to start the microservices.
Start the RabbitMQClient by running the LinqPad script in the root folder (or convert it to a .net core console application.)

Start the API gateway web app by navigating to the `OcelotAPIGateway` and running in with the `dotnet` command line tool. 

You can then make requests through the Gateway e.g. Get https://localhost:PORT/gateway/product

