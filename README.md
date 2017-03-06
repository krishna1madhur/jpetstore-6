
Project Description: Deployed JPetStore, a full-fledged web application on Microsoft Azure Cloud Platform. Explored and analyzed different deployment strategies before deploying it as a cloud service. Did end-to-end performance testing of the app using Apache JMeter. Discovered cloud provisioning strategies that increased the availability, consistency and throughput of the application.

The detailed report regarding the tests that were carried out is at: krishna1madhur/jpetstore-6/Report.pdf 

MyBatis JPetStore
=================

[![Build Status](https://travis-ci.org/mybatis/jpetstore-6.svg?branch=master)](https://travis-ci.org/mybatis/jpetstore-6)
[![Coverage Status](https://coveralls.io/repos/github/mybatis/jpetstore-6/badge.svg?branch=master)](https://coveralls.io/github/mybatis/jpetstore-6?branch=master)
[![Dependency Status](https://www.versioneye.com/user/projects/5619aafaa193340f320005fe/badge.svg?style=flat)](https://www.versioneye.com/user/projects/5619aafaa193340f320005fe)
[![License](http://img.shields.io/:license-apache-brightgreen.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)

![mybatis-jpetstore](http://mybatis.github.io/images/mybatis-logo.png)

JPetStore 6 is a full web application built on top of MyBatis 3, Spring 4 and Stripes.

Essentials
----------

* [See the docs](http://www.mybatis.org/jpetstore-6)

## Other versions that you may want to know about

- JPetstore on top of Spring, Spring MVC, MyBatis 3, and Spring Security https://github.com/making/spring-jpetstore
- JPetstore with Vaadin and Spring Boot with Java Config https://github.com/igor-baiborodine/jpetstore-6-vaadin-spring-boot
- JPetstore on MyBatis Spring Boot Starter https://github.com/kazuki43zoo/mybatis-spring-boot-jpetstore

## Run on Application Server
Running JPetStore sample under Tomcat (using the [cargo-maven2-plugin](https://codehaus-cargo.github.io/cargo/Maven2+plugin.html)).

- Clone this repository

  ```
  $ git clone https://github.com/mybatis/jpetstore-6.git
  ```

- Build war file

  ```
  $ cd jpetstore-6
  $ mvn clean package
  ```

- Startup the Tomcat server and deploy web application

  ```
  $ mvn cargo:run
  ```

  > Note:
  >
  > We provide maven profiles per application server as follow:
  >
  > | Profile   | Description |
  > | --------- | ----------- |
  > | tomcat90  | Running under the Tomcat 9.0 (Mileston version) |
  > | **tomcat85**  | **Running under the Tomcat 8.5 (default profile)** |
  > | tomcat80  | Running under the Tomcat 8.0 |
  > | tomcat70  | Running under the Tomcat 7.0 |
  > | tomee     | Running under the TomEE 7 |
  > | wildfly   | Running under the WildFly 10 |
  > | liberty   | Running under the WebSphere Liberty 16 |
  > | jetty     | Running under the Jetty 9 |
  > | glassfish | Running under the GlassFish 4 |
  > | resin     | Running under the Resin 4 |
  >
  > ```
  > $ mvn cargo:run -P tomcat90
  > ```

- Run application in browser http://localhost:8080/jpetstore/ 
- Press Ctrl-C to stop the server.
