# NodeJs-Website-Docker
Simple NodeJs web with Docker Container
# Build Simple Website with NodeJS, Express & EJS view engine

## Document
* Install dependencies using [npm](https://www.npmjs.com/) javascript package manager: ``` npm install ```
* Start node server with [nodemon](https://nodemon.io/): ``` nodemon start ```
* Tune to url: ``` http://localhost:8080 ```

All boilerplate code managed by [express generator](https://expressjs.com/en/starter/generator.html) framework adhering to DRY rule. Routes are defined in routes/index.js file, static view pages are in views folder. I have implemented partials concept to avoid code redundancy in html using EJS view engine. Css and Javascript files are stored in public folder. 

## Docker

There is a Docker file included with the code
Run the following commands to Build and Run the application within a container.

    ## Build
    docker build --tag zeeshansdocker/nodejs-website:latest . (Please replace 'zeeshansdocker' with your docker accountname)
    ## Run
    docker run --name zeeshansdocker-nodejs-website -p 49160:8080 -d zeeshansdocker/nodejs-website:latest (Please replace 'zeeshansdocker' with your docker accountname)
    
    If all goes well above then you should have the container running in your local Docker install
    Access the website by entering the http://localhost:8080 in your browser




