# ConfigSvcs Configuration Repository

ConfigSvcs is a simple configuration repository that I use for other microservices to store/retieve their configuraiton information.
It makes use of a simple Sqlite3 database to store the configuration JSON blocks, and has a simple API to manage it all.  In theory it
should be scalable by putting a Load Blancer in front of the ConfigSvcs containers, but I haven't had the need to scale it up (most
microservices only need to access the service at startup, or for any config changes, which should be a VERY infrequent occurance.)

