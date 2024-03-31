# ci-cd-example
A simple .NET 6 Web API with a CI/CD pipeline using GitHub Actions and Dockerization.

How to run this project?
- VS: Open the project in VS and build and run. It will open the swagger page with GET enpoint for "CurrentTime". 
    - NOTE: Accept the popup to create self-signed cert

- VS Code: Use dotnet build and run commands. Once it is available on localhost:port, browse for swagger page.
- Docker:
    - docker build -t <image-name> <location-of-docker-file>
    - docker images  #Check for image
    - docker run -p 8080:80 <image-name>
    - Browse for swager page on http://localhost:8080