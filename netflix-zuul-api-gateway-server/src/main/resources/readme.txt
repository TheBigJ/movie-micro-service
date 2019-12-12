Zuul has mainly four types of filters that enable us to intercept the traffic in different timeline of the request processing for any particular transaction. We can add any number of filters for a particular url pattern.

1. pre filters – are invoked before the request is routed.
2. post filters – are invoked after the request has been routed.
3. route filters – are used to route the request.
4. error filters – are invoked when an error occurs while handling the request.	

###########################################################
Some of the common responsibility of gateway service are :
###########################################################

1. Apply microservice authentication and security in the gateway layer to protect the actual services.

2. We can do microservices insights and monitoring of all the traffic that are going in to the ecosystem by enabling 
   some logging to get meaningful data and statistics at the edge in order to give us an accurate  view of production.
   
3. Dynamic Routing can route requests to different backend clusters as needed.
4. We can do runtime stress testing by gradually increasing the traffic to a new cluster in order to gauge performance 
   in many scenarios e.g. cluster has new H/W and network setup or that has new version of production code deployed.
5. We can do dynamic load shedding i.e. allocating capacity for each type of request and dropping requests that go 
   over the limit.
6. We can apply static response handling i.e. building some responses directly at the edge instead of forwarding them 
  to an internal cluster for processing.