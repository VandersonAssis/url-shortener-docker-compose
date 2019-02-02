# Deploy it using docker (EASIER)
This repository has the docker compose yml file that's used to deploy the URL Shortener web application on your server. Please follow the below steps to use it:

- Clone this repository to your PC.
- Open the command line tool and navigate into the directory of the docker-compose.yml.
- Run "docker-compose up" command.

Please wait until the database container is up, it takes up to two minutes. After it is up, access the application on this url http://localhost:15000/shortener.

# Deploy it manually (YOU'LL GONNA GET HURT)
Of course, to run the application using the above method, you'll have to have Docker installed in your machine, but if you don't have it or don't want it, then just follow the following steps.

- Have tomcat 8.5, java8 and mysql8 installed on your PC.
- Clone the api project https://github.com/VandersonAssis/url-shortener-api.
- Clone the client project https://github.com/VandersonAssis/url-shortener-client.
- In the client project, you'll see a file called shortener.war, just copy it into your tomcat's webapps directory and then start it.
- Execute the api's database_initialization.sql file on your mysql8 engine.
- In the api project, you'll also see the shortener-api.jar. Just double click it and the api will be up to go.

# Coming up next...
- Secure the api using OAuth2.0

For info on how to use this application, please follow this link https://github.com/VandersonAssis/url-shortener-client.

My DockerHub page is https://hub.docker.com/u/vandersonassis.
