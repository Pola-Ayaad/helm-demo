# Deploy python app using Helm 

1- Cloning the repository Git clone https://github.com/tradebyte/DevOps-Challenge.git
2- Creating DockerFile 
3- Building DockerFile Docker build -t (image name)
4- login to your dockerhub docker login --- enter your user name and password 
5- docker images 
6- docker tag (image id) (your dokcerhub username)/(image name):(tag name)
7- docker push (your dokcerhub username)/(image name):(tag name)
8- create chart.yaml
9- create values.yaml
10- create templates folder that will have the deployment and services files 
11- create the app helm create (name)
12- run minikube --- minikube start 
13- install your app --- helm install (release name) (image name)
14- get the ip of your application --- kubectl describe no minikube | grep -i InternalIP 
15- go to your browser enter the IP:30009
