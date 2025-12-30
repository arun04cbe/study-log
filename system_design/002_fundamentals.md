# Some Fundamentals which is used for communication between client and server

1. `Polling`
2. `Long Polling` - Hanging GET
   1. Client sends the requests and the server does not immediately respond.
   2. Instead it holds the request until some changes happen and then sends the response
   3. If there are no changes, the connection gets timed out and a new connection is created.
3. Cons with Polling
   1. At a certain periodic interval a new connection is created.
   2. This makes the operations bit costly.
4. `Web Sockets` on the other hand keeps the connections unique, where server can share the data with the client
   1. Stream messages independently
   2. Asynchronous
   3. Apps
      1. Gaming Apps
      2. Real Time Apps - Stock Trading
      3. Chat Apps
