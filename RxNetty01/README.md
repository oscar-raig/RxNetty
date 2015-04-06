## Simple RxNettyServer Example

The program start a server.



, if the uri ("request.getPath()") is /error,
( http://localhost:8080/error ) throws an exception and we return
response.setStatus(HttpResponseStatus.BAD_REQUEST);



### Building and Run

```
gradle runHelloWorldClient
````

Output 

````
Server => Request: /
Client => Path Requested =>: /

Server => Request: /error
Server => Error [/error] => java.lang.RuntimeException: forced error
Client => Error 500: Bad Request

Server => Request: /data
Client => Path Requested =>: /data

````

