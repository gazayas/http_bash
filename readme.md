#http

A command line tool for looking up http statuses

##Installation
`$ curl -o /usr/local/bin/http https://raw.githubusercontent.com/gazayas/http/master/http` <br/>
`$ chmod 755 /usr/local/bin/http`

##Usage
```
$ http 200
200 OK

$ http 100 200 404
100 Continue
200 OK
404 Not Found

$ http 417 -d  #For details
417 Expectation Failed
The server cannot meet the requirements of the Expect request-header field.

$ http 200 404 503 -d  #Details for multiple statuses can be looked up all at once

$ http -l  #for the master list
100 Continue
101 Switching Protocols
102 Processing
200 OK
201 Created
202 Accepted
...
```
