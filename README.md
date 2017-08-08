# elastic-beanstalk-tutorial
Example application using Docker to deploy with Elastic Beanstalk
These two blog posts make use of this sample application:
  * [Deploying a Docker Container with AWS Elastic Beanstalk](https://medium.com/@sommershurbaji/deploying-a-docker-container-to-aws-with-elastic-beanstalk-28adfd6e7e95)
  * [Continuous Delivery with AWS Elastic Beanstalk](https://medium.com/@sommershurbaji/continuous-delivery-with-aws-elastic-beanstalk-and-travis-ci-2dd54754965f)

### Build Status: [![Build Status](https://travis-ci.org/sommercodes/elastic-beanstalk-tutorial.svg?branch=master)](https://travis-ci.org/sommercodes/elastic-beanstalk-tutorial)

# Set Up Instructions

* clone:
`git clone https://github.com/sommercodes/elastic-beanstalk-tutorial.git`
* install dependencies: `npm install`
* start server: `npm start`
* navigate to http://localhost:8080

# Docker Instructions:
* To build a docker image of the app, in your terminal, navigate to the app's root directory and run: `docker build -t eb-tutorial .`
* To run a docker container of the image you just build, run the command: `docker run -d -p 8080:8080 --name eb-tutorial eb-tutorial`
* Use the command `docker ps` to make sure your container is running

* If you are on mac or linux, navigate to http://localhost:8080 in your browser to view your running app.
* If you are on windows, navigate to http://\<**port docker runs on**\>:8080 in your browser to view your running app.


