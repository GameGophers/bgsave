# redis persistence service
[![Build Status](https://travis-ci.org/GameGophers/bgsave.svg?branch=master)](https://travis-ci.org/GameGophers/bgsave)

dump records from redis.      
the format of the record is defined as :         

key(tablname:record_id) -> value(packed)

# environment variables:
* REDIS_HOST : eg: 127.0.0.1:6379    
* MONGODB_URL : eg: mongodb://172.17.42.1/mydb
* NSQD_HOST :  eg: http://172.17.42.1:4151

# install
install gpm, gvp first        
$go get -u https://github.com/GameGophers/bgsave/        
$cd bgsave     
$source gvp        
$gpm       
$go install bgsave         

#install with docker
docker build -t bgsave .     
