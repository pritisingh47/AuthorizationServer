# AuthorizationServer
Authorization server implemented using Spring security oauth2 framework.
database used : H2 db

# How to use it
Follow the below steps in order to make rest endpoints secure:
* Clone the AutorizationServer and make it run.
* In any other project which has to make secure, add outh2 and security dependency in pom.
* Annotate the main class with EnableResourceServer annotation.
* and last, add the following properties in application.properties file 
security.oauth2.resource.token-info-uri=http://localhost:9090/oauth/check_token
security.oauth2.client.client-id=mobile
security.oauth2.client.client-secret=pin

