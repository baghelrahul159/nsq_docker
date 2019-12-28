# nsq_docker
Docker Compose for NSQ

Compose file consist of 3 docker containers required for setting up nsq.
* NSQLookupd
* NSQd
* NSQadmin

### nsqlookupd 
is the daemon that manages topology information and provides an eventually consistent discovery service.

### nsqd 
is the daemon that receives, queues, and delivers messages to clients.

### nsqadmin 
is a web UI to introspect the cluster in realtime (and perform various administrative tasks).

Please note that options lookupd-tcp-address and broadcast-address are very important for containers to allow each other to communicate and to allow localhost to communicate with containers.