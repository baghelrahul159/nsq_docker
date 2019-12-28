# nsq_docker
Docker Compose for NSQ

Compose file consist of 3 docker containers required for setting up nsq.
1. NSQLookupd
2. NSQd
3. NSQadmin

1. nsqlookupd is the daemon that manages topology information and provides an eventually consistent discovery service.
2. nsqd is the daemon that receives, queues, and delivers messages to clients.
3. nsqadmin is a web UI to introspect the cluster in realtime (and perform various administrative tasks).

Please note that options lookupd-tcp-address and broadcast-address are very important for containers to allow each other to communicate and to allow localhost to communicate with containers.