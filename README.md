# Recipes-Management-Search-System
Please do not use any VPN as it might not connect to hosted kafka.

This is a combination of three microservices.
Recipes-Authoring-Command-Service→1 Handling all CRUD APIs and sending data to Kaka Queue.
Recipes-Search-Consumer-Service→2 Consuming Kafka queue and indexing in Elastic search.
Recipes-Search-Service→3 Searching in Elastic Search.
For Fast searching, I used Elastic Search.
For async processing→ Kafka.
It is production ready→ as we can do the scaling of any of the MS based on the traffic received.
