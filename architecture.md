## Architecting of infrastructure, applications and services.

**Project description:** I have worked as a software engineer on numerous projects requiring overall system design, architecting cloud services for a myriad of industries, also writing big-data applications which have tons of variation in how the data is delivered, presented, and memory constraints.  Here is a few projects that were worth delving into:



### 1. Consumer facing, high volume microservices on AWS.

As a fullstack engineer on a project with incoming messages on order of 10k+ per min.  All components needed to be auto-scaling to handle traffic during peak hours, and be fault-tolerant.  
Java handles the heavy lifting; after the kinesis event stream is split into a database of event logs and a NoSQL store for current device state.  
The modular cloud components are easy to deploy, and services are trivial to stop/start, and CloudWatch was an essential component to catch any failures, and create audits of daily activity. 
A local kinesis build was included in the CI/CD paradigm for faster development.  
The infrastructure rollout looks like this:

```
API Gateway
Kinesis streams
Redshift
Internal API
PostgreSQL Warehouse
```

<img class='feature'  src="images/jacloud.jpg?raw=true"/>

<br>
---

### 2. Big-data and stream processing architectures and workflows.
A bulk-data processing system, as contracted by a large insurance company.  Its purpose is to run a daily aggregation against the internal data warehouse, and comb through the claims in order to detect fraud, descrepancies, and a myriad of other causes of faulty data.  This architecture is built with open-source in-mind, using Hive, Spark, SOLR in-memory store, and Java to create large sets of data that could be read from memory, and processed in the period of only a few hours.
Using the knowledge gained from this project, we would eventually expand the functionality into a more robust, modular system.  These modules were enhanced to handle more schama-types, modularized, dockerized, and communicate via a Kinesis messaging hub. A system still in-use to this day. 
Overview:
 
 ```
Spark
Hive
SOLR
Java
Kinesis Streams
Confluent/Open-source
```

<img class='feature' src="images/humid.jpg?raw=true"/>
<br>
---


### 3. Events based services and data flow.
Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 
 
 ```javascript
API Gateway
Kinesis streams
NoSQL
```

<img class='feature' src="images/candc.png?raw=true"/>
<br>
---

### 4. Frontend UI/UX

Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 
 
 ```javascript
API Gateway
Kinesis streams
NoSQL
```
 <img class='feature' src="images/frontend2.jpg?raw=true"/>
 
 
 <style>
.feature{
    border: 1px solid silver !important;
}
</style>