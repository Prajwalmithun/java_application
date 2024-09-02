# Spring Boot (Java) + maven (build) 

## Option 1 : How to run the application ?(locally)

### Step 1: Clone the repository

Either Click on Code -> Open with Github Desktop or 

run the following command in your terminal

```
# git clone https://github.com/Prajwalmithun/java_application.git
# cd java_application
```

# Install "Springboot extention pack" and "Extention pack for Java" in VS code

# Install maven in your system
```
# brew install maven
```

### Step 3: Build the application

```
# mvn clean install
```

### Step 4: Run the application

```
# java -jar target/spring-boot-app.jar
```

### Step 4: Access the application

Open your browser and go to http://localhost:8080


## Option 2: How to run the application on Docker ?

### Step 1: Clone the repository

Either Click on Code -> Open with Github Desktop (OR) run the following command in your terminal

```
# git clone https://github.com/Prajwalmithun/java_application.git
# cd java_application
```

### Step 2: Build the Docker Image

```
# docker build --platform=linux/amd64 -t <DOCKERHUB_USERNAME>/java_application .
```

### Step 3: Run the Docker Container

```
# docker run -dit -p 8080:8080 java_application
```

### Step 4: Access the application

Open your browser and go to http://localhost:8080


### Push the Docker Image to Docker Hub

```
# docker login
# docker push <DOCKERHUB_USERNAME>/java_application
```
Check your dockerhub repository for the image


### Deployment architecture

