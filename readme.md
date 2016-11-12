#http

A command line tool for looking up http protocols

##Installation
`curl -o /usr/local/bin/http https://raw.githubusercontent.com/gazayas/http/master/http`

##Usage
```
$ bin/bash/ http 200
#=> 200 OK

# master list
$ bin/bash/ http -l
#=>
100 Continue
101 Switching Protocols
102 Processing
200 OK
201 Created
202 Accepted
...
```
