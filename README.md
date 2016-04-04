# Multi-threaded-scheduler
Node.js multi-threaded scheduler

### Install
`$ npm install`

### Run:

Run with parameters:

`$ node server.js domain port requestURL -t numberOfThreads -i pollIntervalInSeconds`

---

example:

`$ node server.js localhost 9000 getUserData -t 3 -i 10`


This will command the server to create 3 threads which will make a HTTP GET request to

**http://localhost:9000/getUserData** repeatedly at an interval of 10 seconds.

The parameters **-t** and **-i** are optional, if not specified use default values as:

numberOfThreads = **number of CPU cores**

pollIntervalInSeconds = **5**