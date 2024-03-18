# Documentation

## Development used tools:

 - Go 1.21
 - Gin Gonic v1.9.1
 - Wire v0.5.0
 - Swaggo v1.6.0

## Startup :vertical_traffic_light:

For run the project in localhost you can follow this steps:

- Use `make run` for start the project without update the Wire files
- The execution at home has been disabled, to enable it, lines 48 to 59 must be decomned and the methods comment init, Handler y main, for default, Gin will open the service on `http://localhost:8080` and the Swagger on `http://localhost:8080/swagger/index.html` 

Otherwise if you has made changes in the project you can use this commands:

- Use `make generate` from the project root for generate the dependencies with Wire
- Use `make swagger` from the project root for generate the Swagger Documentation
- Use `make all` (recommended) is the plus between `make generate` `make swagger` and `make run`
- Use `make test` for test the `GetLocation` and `GetMessage` methods
