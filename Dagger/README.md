# Dagger DNS Server

Dagger is a MicroServices-based architecture for a DNS Server that has a REST API for managing entries.   I use this in my labs, so not sure yet about how well it scales.

Dagger is composed of two microservices:  One is a DNS server used to handled DNS Queries on port 53.  Scaling can be achieved by using a
Load Balancer capabile of handling port 53 traffic.  The other microservice is the API service.   Both of these microservices make use of
the ConfigSvcs to store/retrieve their configuration information, as well as a database microservice.
