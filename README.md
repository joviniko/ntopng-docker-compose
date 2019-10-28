# ntopng-docker

[ntopng official site](http://www.ntop.org/products/traffic-analysis/ntop/)  
[User’s Guides](http://www.ntop.org/support/documentation/documentation/)  

Docker Compose is used to analyze traffic from a MikroTik router as described in the [article](http://www.ntop.org/ntopng/how-to-analyse-mikrotik-traffic-using-ntopng/)

## Deployment

### Ports
 - 3000/TCP - ntopng web interface
 - 2055/UDP - nprobe NetFlow/IPFIX/sFlow collector flows port

### Command Line
 ```
docker-compose up -d
 ```

 ### Web UI

 http://127.0.0.1:3000  
 username: admin  
 password: admin  

## Installed packages:
```
ntopng                     3.9.191015
ntopng-data                3.9.191015
nprobe                     8.7.191015-6644
pfring                     7.5.0-2713
pfring-dkms                7.5.0
```