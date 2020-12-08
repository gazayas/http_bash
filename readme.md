There is a better version of this at [gazayas/httpd](http://www.github.com/gazayas/httpd).<br/>
Please use that command line tool instead

# http

A command line tool for looking up http statuses

## Installation
`$ curl -o /usr/local/bin/http https://raw.githubusercontent.com/gazayas/http_bash/master/http` <br/>
`$ chmod 755 /usr/local/bin/http`

## Usage
```
$ http 200
200 OK

$ http 100 200 404
100 Continue
200 OK
404 Not Found

# there are 3 options, and they can all be used together
# -d for details
# -l for the master list
# -jp for Japanese

$ http 417 -d
417 Expectation Failed
The server cannot meet the requirements of the Expect request-header field.

# Details for multiple status can be looked up all at once
$ http 200 404 503 -d

$ http -l
100 Continue
101 Switching Protocols
102 Processing
200 OK
201 Created
202 Accepted
...

# The master list with details
$ http -l -d
```

