# Environment variables

* MONGODB_CONNECTION_URL: Connection URL to mongo database (For example, mongodb://mongo.host:27017/genieacs)
* REDIS_HOST
* REDIS_PORT
* CWMP_INTERFACE: Interface where CWMP server is going to bind (default 0.0.0.0)
* CWMP_PORT: default 7547
* CWMP_SSL: True or False, activate or not SSL
* NBI_INTERFACE: Interface where NBI server is going to bind
* NBI_PORT: default 7557
* FS_INTERFACE: Interface where FS server is going to bind
* FS_PORT: default 7567
* FS_IP
* LOG_IMFORMS
* DEBUG

MONGODB_CONNECTION_URL and REDIS_HOST are the only two environment variables you need to use, all the rest are optional.

# Example usage

```
# docker run --name genieacs-server \
    -e MONGODB_CONNECTION_URL=mongodb://mongo.host:27017/genieacs \
    REDIS_HOST=redis.host -p 7547:7547 \
    -d genieacs
```
