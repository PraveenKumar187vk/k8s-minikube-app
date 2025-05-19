
# Kubernetes Minikube Demo

## Task 5 - DevOps Internship
**Objective:** Deploy and manage a simple NGINX app in Kubernetes using Minikube.

---

## Tools Used
- Minikube
- kubectl
- Docker

---

## Steps

1. **Start Minikube**
    ```bash
    minikube start
    ```

2. **Deploy Application**
    ```bash
    kubectl apply -f deployment.yaml
    ```

3. **Expose the Application**
    ```bash
    kubectl apply -f service.yaml
    ```

4. **Verify and Scale**
    ```bash
    kubectl get pods
    kubectl scale deployment nginx-deployment --replicas=3
    kubectl get pods
    ```

5. **Logs and Describe**
    ```bash
    kubectl describe pod <pod-name>
    kubectl logs <pod-name>
    ```

---

## Output

### Pods
![Pods](./screenshots/pods.png)

### Services
![Services](./screenshots/services.png)

### Describe Pod
![Describe](./screenshots/describe_pod.png)

---

## Outcome
> Learned how to deploy and manage Kubernetes workloads locally with Minikube.
