# monitoring-docker-compose

## Start and Stop
Start
```
docker-compose up -d --build
```
Stop
```
docker-compose down
```

shot jenkins initalAdminPassword
```
docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword
```

## URL  
- Jenkins  
http://localhost:8080  

- prometheus  
http://localhost:9090  

- grafana  
http://localhost:3000  

- redmine  
http://localhost:3030  
