# Microservices

Sample architecture for grouping several microservices. For clarity we'll assume we're making a simple chat application.

Following are the microservices:

1. **Authentication** This service deals with creation and deletion of authentication token that can be used across various other services to validate the authenticity of the client.

2. **Resource** To supply html/js/css to the client on request/load.

3. **Database** To be used internally by other services to store and retrieve data.

4. **API Gateway** The only service client will directly interact with. This will then redirect the request to its associated services as per the clients request.

5. **Members** To perform CRUD on the members.

6. **Groups** To perform CRUD on the groups.

7. **Messages** To perform CRUD on messages passed on between the application.

8. **Socket** To maintain the socket pool providing the online status of the members. 


