# oneWeb docker image	

Minimal docker image for oneweb tomcat installation.


### Prerequisites ###

* Install [docker](http://docs.docker.com/mac/step_one/).


### Quick Start ###

* Clone this repo.
* Download the oneweb-tomcat-sdk from [Nexus](https://maven.onewebuxp.allianz/index.html#nexus-search;gav~com.allianz.oneweb~com.allianz.oneweb.sdk.tomcat~feature-OW-2406-tomcat-SNAPSHOT~~).
* Built the docker imager: `docker build -t oneweb:latest .`.
* Run the docker container from the image: `docker run --name oneweb -p 8081:8081 oneweb:latest`.


### Notes ###

The image can later on stopped and started with `docker stop oneweb` and `docker start oneweb`.


