# k8s-session

#1 Start a webserver
go run hello.go

#2 Build a docker image
sudo docker build -t ust-hello:v1

#2 Start a webserver from a docker image
sudo docker run -it --rm -p 80:80 --name my-running-app ust-hello:v1


#3 Build the docker image, to push to public docker repo
sudo docker build -t veeshall/ust-hello:v1
sudo docker push veeshall/ust-hello:v1

#4 Create a kubernetes Cluster in GCP


#5 Deploy the image in GKE
# Do a perf test to verify Auto scaling
ab -n 10000 -c 100 http://35.222.8.155/ust-team

#6 Deploy the image in tmo cluster



