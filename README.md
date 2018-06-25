# devops-test-helloworld-app

This folder contains the sample code for a Spring boot application used for the devops technical test. See the instructions below for how to deploy and run this application.

[ci-badge]: https://storage.googleapis.com/nodejs-getting-started-tests-badges/1-tests.svg

# Dependencies
This Application needs a PostgresSQL database. Version 9.6 or higher is required. For development environment a docker-compose is provided within this project.

# Run application

### Dev environment

1. Go to the application directory
2. `docker-compose up`
3. `./gradlew run`

### Prod environment

1. Build the application: `./gradlew build`. This command will generated the following jar: `build/libs/helloworld-0.0.1-SNAPSHOT.jar`
2. Run the application: `java -jar helloworld-0.0.1-SNAPSHOT.jar --spring.profiles.active=pro`

