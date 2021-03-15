# java-web-gradle-spring-websocket-secure-des-encoded-thyme-vanilla

## Description
This is a gradle built springboot web app
using the STOMP subprotocol to communicate
over websockets to vanilla javascript thymeleaf clients.
By clients, we mean any number of visitors to
this website will see changes in real time.
  Security was added so that the insecure page `/login` will
be redirected to when hitting a secure page. DES was used
to encrypt and BCrypt to encode the password.
  The project is simple, the visitor clicks a
button which is updated on the server as well as
a log. Any new visitor will receive all logs and
an updated click count.

## Tech stack
- java
- maven
  - springboot
  - thymeleaf
  - bootstrap
  - jquery
  - sockjs

## Docker stack
- gradle:jdk11

## To run
`sudo ./install.sh -u`
Available at http://localhost
Login with id: user and password: pass

## To stop (optional)
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
- http://makble.com/build-groovy-project-with-gradle
- https://www.marcelustrojahn.com/2015/11/spring-boot-groovy-gradle-hello-world-application/
