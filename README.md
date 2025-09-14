# Kubernetes-Deployment-and-Scaling
This project outlines a series of tasks focused on deploying, managing, and scaling an application on a Kubernetes cluster. The process covers creating deployment and service manifests, deploying the application, and performing scaling and rolling updates.

# Task 1: Select a Sample Application
We used a simple web application, an Nginx server, which is lightweight and easy to deploy. We also learned how to customize the application by adding a simple webpage or a status endpoint.

# Task 2: Environmental Setup
Before deployment, we ensured we had access to a local Kubernetes cluster using Minikube and that kubectl was properly installed and functioning to interact with the cluster.

# Task 3: Create Deployment Manifest
A YAML file was created to define a Kubernetes Deployment for our application. This manifest specifies the container image to use, the desired number of replicas, and the ports to expose.

# Task 4: Expose the Application
A separate Service YAML file was created to expose the deployment externally. We used a NodePort or LoadBalancer service type to enable access from outside the cluster.

# Task 5: Deploy and Test
The application and service were deployed using the kubectl apply -f <file.yaml> command. We validated the successful deployment by checking the status of the pods and verifying that the application was running.

# Task 6: Scaling and Update Exercise
We practiced scaling the deployment up or down using the kubectl scale command. We also performed a rolling update by changing the container image tag to a newer version, ensuring the update was completed without any service downtime.

Learnings and Conclusion
This project provided hands-on experience in several key areas of Kubernetes:

Deployment and Service Manifests: Writing and applying YAML configurations to define application components.

Scaling: Understanding how to scale an application to handle increased load and the effects of scaling on application performance and resource usage.

Rolling Updates: Performing zero-downtime updates by incrementally replacing old pods with new ones.

Troubleshooting: Gained experience in debugging common issues, such as a pod not creating properly, by restarting Minikube and re-applying configurations.
