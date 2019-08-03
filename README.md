# monitoring-docker-compose

docker run -d --rm --name jenkins -p 8080:8080 -p 50000:50000 jenkins/jenkins
docker run -d --rm --name prometheus -p 9090:9090 -v /Users/yurak/dev/logging/prometheus.yml:/etc/prometheus/prometheus.yml prom/prometheus
docker run -d --rm --name grafana -p 3000:3000 grafana/grafana

## Start and Stop
Start
```
docker-compose up -d --build
```
Stop
```
docker-compose down
```

docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword

URL  
http://localhost:8080
http://localhost:9090
http://localhost:3000

