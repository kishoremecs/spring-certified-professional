# List of Contents

### Example 1 Describes a Basic Authentication enabled with default configuration in Spring Boot.

## Helpful Commands

openssl req -newkey rsa:2048 -x509 -keyout key.pem -out cert.pem -days 365
openssl pkcs12 -export -in cert.pem -inkey key.pem -out certificate.p12 -name "certificate"


## Enabling HTTPS in Spring Boot
server.ssl.key-store-type=PKCS12
server.ssl.key-store=classpath:certificate.p12
server.ssl.key-store-password=12345  

