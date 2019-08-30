# spring-samples-soap-webservice
Test app with a SOAP service

App was created by a guide: https://spring.io/guides/gs/producing-web-service/

# How to run:

1) Run the application using ./mvnw spring-boot:run. 
2) Or you can build the JAR file with ./mvnw clean package. Then you can run the JAR file:
java -jar target/gs-soap-service-0.1.0.jar


# Simple request:

<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
				  xmlns:gs="http://spring.io/guides/gs-producing-web-service">
   <soapenv:Header/>
   <soapenv:Body>
      <gs:getCountryRequest>
         <gs:name>England</gs:name>
      </gs:getCountryRequest>
   </soapenv:Body>
</soapenv:Envelope>