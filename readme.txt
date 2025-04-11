docker login
kubectl get nodes                                                                        (verify k8s)
kubectl get deployments                                                                  (verify k8s)
kubectl get pods --all-namespaces                                                        (verify k8s) 
kubectl port-forward svc/homeverse-service 8081:80                                       (to run kubernetes)    
kubectl get secret grafana -o jsonpath="{.data.admin-password}" | base64 --decode; echo  (to get password for grafana. username: admin)
kubectl port-forward svc/grafana 3001:80                                                 (to run grafana)
docker run -p 8081:80 homeverse-app:v1                                                   (to run docker containers)


