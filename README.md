systemctl start docker

docker ps

docker pull infracloudio/csvserver:latest

docker pull prom/prometheus:v2.22.0

git clone https://github.com/infracloudio/csvserver.git

docker run -d -p 9393:9300 -v /root/inputFile:/csvserver/inputdata infracloudio/csvserver:latest
vi gencsv.sh

chmod 755 gencsv.sh

./gencsv.sh 10

ls

cat inputFile

docker run -d -p 9393:9300 -v /root/inputFile:/csvserver/inputdata infracloudio/csvserver:latest

docker exec -it {containerid} bash 

sudo netstat -tulpn | grep LISTEN

docker kill {containerid}

docker run -d -p 9393:9300 -e CSVSERVER_BORDER=Orange -v /root/inputFile:/csvserver/inputdata infracloudio/csvserver:latest

touch README.md

echo "docker run -d -p 9393:9300 -e CSVSERVER_BORDER=Orange -v /root/inputFile:/csvserver/inputdata infracloudio/csvserver:latest" > part-1.cmd

curl -o ./part-1-output http://localhost:9393/raw

docker logs [container_id] >& part-1-logs












