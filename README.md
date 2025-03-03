Spring Boot REST Controller Setup:
1. Created a HelloController with REST endpoints using @RestController and @RequestMapping("/hello").
Implemented a PUT API that takes firstName as a Path Variable and lastName as a Query Parameter.
cURL Request for Testing
2. Used curl -X PUT "http://localhost:8080/hello/put/Prashant?lastName=Bhadoria" -w "\n" to test the API.
Fixed the 404 error caused by an extra / before the query parameter.

3. Expected Output & Debugging Steps
    API should return: "Hello Prashant Bhadoria from BridgeLabz".
    Verified application is running (mvn spring-boot:run), ensured proper controller setup, and corrected the cURL request.