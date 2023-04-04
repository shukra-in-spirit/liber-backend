# liber-backend
Liber is the patron of the Plebius in Roman mythology. Under his auspices the common Romans, wined, dined and enjoyed. The project named after him creates a group based chat application, where users can create groups, chat in them and post updates about their life in feeds. This repository contains the various microservices which cumulatively provide the backend for the liber application.

## Microservices

### Seneca (Not yet started) (1st)
Seneca was celebrated as a sage, for his morals, wisdom and knowledge. Seneca is a <strong>datastore microservice</strong>. It will be interacting with AWS Dynamodb for maintaining the data on groups, users, feed, and credential information that the liber application generates. It provides a grpc interface for a faster delivery of information.
<br><br>

### Carthage (Not yet started)
The bitter rivalry with Carthage was the test of Rome. It is a <strong>html, javascript based mock UI</strong> which will be used for testing and ensuring the functionality of the backend. As we are following a TDD pattern. Carthage will be updated to test for the feature before the feature is implemented. It will be performing integration and scale testing.
<br><br> 

### Ceasar (Not yet started)
Julius Ceasar is one of the most accomplished and popular generals of Rome. His conquests are celebrated in our <strong>group-based chatting service backend</strong>. Ceasar uses web-sockets to interact with the client applications. There is one socket per user. On event for that user, the client application senses the group where the event belongs and updates accordingly.
<br><br>

### Colosseum (Not yet started)
The Amphitheatre where Romans crowded for entertainment. The <strong>backend for the feed</strong> is utilizing a grpc mechanism to serve data to the feed at the home page of the liber application.
<br><br>

### Praetor (Not yet started)
One of the ranks of the Roman judicial officers. It will serve as a <strong>RBAC broker for CRUD user/group-admin/support permissions</strong>. It will be based on the OAPI service broker architecture. Permissions and roles for all the users of the application is maintained here. Tokens valid for one day can be obtained here for authenticating for the secure endpoints.
