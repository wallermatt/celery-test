# celery-test

https://docs.celeryq.dev/en/stable/getting-started/first-steps-with-celery.html#first-steps

brew install redis

redis-server

brew services start redis
brew services info redis
brew services stop redis

redis-cli
https://redis.io/docs/manual/cli/

$ redis-cli <command>

SET mykey "Hello"
GET mykey

INCR intkey


by default connects to 127.0.0.1 6379

redis-cli -h redis15.localnet.org -p 6390 

PING


redis-cli -a myUnguessablePazzzzzword123 PING << if redis instance password protected
REDISCLI_AUTH

-n database number?


--tls --cacert  --cacertdir enable SSL/TLS

$ redis-cli -x SET net_services < /etc/services
OK
$ redis-cli GETRANGE net_services 0 50
"#\n# Network services, Internet style\n#\n# Note that "

SELECT <db num>

CONNECT <different instance>

HELP

HELP @<category> shows all the commands about a given category. The categories are:
@generic
@string
@list
@set
@sorted_set
@hash
@pubsub
@transactions
@connection
@server
@scripting
@hyperloglog
@cluster
@geo
@stream


redis-cli --stat

redis-cli --bigkeys

redis-cli MONITOR

https://redis.io/docs/manual/pubsub/

