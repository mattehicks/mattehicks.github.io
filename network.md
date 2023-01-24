## A network manager, command and control platform, and CMS all-in-one.

**Project description:** This was a project that took 2 years to complete.  
Consisting of multiple UI/UX interfaces, complex business-objects, multiple programming languages, critical services, authentication methods, 
databases, API's and microservices, and python/java data-analysis modules running in the background.
It was able to interface with remote "edge-devices" and local network hardware. Each with a hand-written modular interface for each protocol or interface required.

### 1.  Interface design
Initial concept was built with vanilla Javascript, including a very dynamic page loading context.  CRUD components were built to utilize internal APi's for adding/deleting entities, and permissions for users.   A mapping framework was used to display realtime telemmetry of field units, with dropdowns multiple layers of interactions and labelling.  
Upon successful demo of the application, funding was secured to improve the interface with more modern components and frameworks, like Angular and Typescript.

``` 
GRPC subscriber and socket communications.
TCP/IP, Socket, UDP and SMTP messaging.
CMS CRUD capabilities.
Secure: Tokenized/authenticated application interface.
```
<img src="images/network1.png?raw=true"/>


### 2. Programming and methods

The core components written in Java; utilizing singletons, realtime contexualized data from MongoDB and MySQL.
Deployed using Wildfly and Containers, in a private environment.
Python services ran as a glue component between 3rd party monitoring software in order to aggregate and shuffle realtime input with stored database entity objects.
Data analysis was achieved with ELK (Elasticsearch, Logstash, Kibana).
Realitime dashboards and graphing was done with COTS 3rd party tools.
 
<img src="images/network2.png?raw=true"/>