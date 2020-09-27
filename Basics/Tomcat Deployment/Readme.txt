Steps:

1. Define the Deployment 
   - Indicates what image to use and what services that image exposes
   - Command: kubectl apply -f deployment.yaml
   
2. Expose its services
   - Map those exposed services to from the container to the outside world.
   - Ask Minikube which port it is using for this.
   - Commands: 
        kubectl expose deployment tomcat-deployment --type=NodePort
        minikube service tomcat-deployment --url

3. Deploy it to our Cluster
