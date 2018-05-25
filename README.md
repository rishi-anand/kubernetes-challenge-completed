# Kubernetes Challenge

### Question
![Alt text](resources/question.png?raw=true "Title")


### Solution
Verify the solution by navigating to below endpoint.

## [http://35.201.127.175](http://35.201.127.175)
> &#x1F538;**Note:** Above endpoint is not accessible as this deployment and other related resources was deleted at 00:00 Hrs on 22nd May 2018 to reduce carbon footprints. 
> 
> &#x1F34F;<span style="color:Green;"><b>Go Green</b></span>&#x1F34F;


![Alt text](resources/success_message.png?raw=true "Title")

### Steps to build DockerFile and upload image to docker hub
1. Build docker image.
    ```sh
    $ docker build -t kubernetes-challenge .
    ```
2. Add tag in image based on username and docker respository.
    ```sh
    $ docker tag kubernetes-challenge rishianand/k8s:base
    ```
3. Upload image to docker hub.
    ```sh
    $ docker push rishianand/k8s:base
    ```
    
### Deploy below yaml file(s) in k8s 

I have deployed below yaml files.

| Yamls | Link |
| ------ | ------ |
| Service | https://github.com/rishi-anand/kubernetes-challenge-completed/blob/master/service-nodeport.yaml |
| Ingress | https://github.com/rishi-anand/kubernetes-challenge-completed/blob/master/ingress.yaml |
| Config Map | https://github.com/rishi-anand/kubernetes-challenge-completed/blob/master/config_map.yaml |
| Deployment | https://github.com/rishi-anand/kubernetes-challenge-completed/blob/master/deployment.yaml|

