# dumb
A dumb HTTP server

# Build
```
go build
```

# Run
```
./dumb &
```

# Benchmark with Apache Benchmark

```
➜ time ab -n 100 -c 100 http://localhost:8080/bar
This is ApacheBench, Version 2.3 <$Revision: 1706008 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking localhost (be patient).....done


Server Software:        
Server Hostname:        localhost
Server Port:            8080

Document Path:          /bar
Document Length:        13 bytes

Concurrency Level:      100
Time taken for tests:   0.514 seconds
Complete requests:      100
Failed requests:        0
Total transferred:      13000 bytes
HTML transferred:       1300 bytes
Requests per second:    194.54 [#/sec] (mean)
Time per request:       514.044 [ms] (mean)
Time per request:       5.140 [ms] (mean, across all concurrent requests)
Transfer rate:          24.70 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        1    3   1.2      3       5
Processing:   506  507   0.4    507     508
Waiting:      506  507   0.4    507     508
Total:        507  511   1.3    510     513

Percentage of the requests served within a certain time (ms)
  50%    510
  66%    511
  75%    512
  80%    512
  90%    513
  95%    513
  98%    513
  99%    513
 100%    513 (longest request)

real	0m0.572s
user	0m0.008s
sys	0m0.048s
```

# Brilliant!
