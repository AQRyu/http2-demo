
# Demo for HTTP2 Spring boot application

This project is to demonstrate how to implement h2 protocol to Spring boot application in the local development environment

# Requirements

- jdk 11
- mkcert (refs to https://github.com/FiloSottile/mkcert)

# Installation

- Generate the p12 key:
  ```
  mkcert -pkcs12 localhost 127.0.0.1 ::1
  ```
  > This creates a new file localhost+2.p12 in the current directory. The PKCS#12 bundle is secured with the password changeit.
  
- Copy the generated key to /resources

- Start the application from the command line or inside your IDE.
  ```
  ./mvnw spring-boot:run
  ```