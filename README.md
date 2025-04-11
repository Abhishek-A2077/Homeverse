# HomeVerse

HomeVerse is a cutting-edge real estate platform designed to streamline property exploration, showcase detailed listings, and connect users with realtors effortlessly. Built with HTML, CSS, and JavaScript, it delivers a seamless, interactive, and user-friendly browsing experience, making house hunting more intuitive than ever. 

## Features  
- 🏠 **Browse Properties** – View detailed property listings with images and descriptions.   
- 📞 **Contact Realtors** – Easily connect with property owners or agents.  
- 📱 **Responsive Design** – Optimized for mobile and desktop viewing.    

## Technologies Used  
- **HTML** – Structuring the webpage  
- **CSS** – Styling and layout  
- **JavaScript** – Interactive features  

## Live Demo  
🔗 **Visit HomeVerse:** [HomeVerse Website](https://abhishek-a2077.github.io/Homeverse/)  

## Preview  
![HomeVerse Preview](assets/images/homeverse%20preview.jpg)

# 🚀 Instructions to Run Docker, Kubernetes, and the Cloud Native Monitoring Dashboard (Made with Prometheus and Grafana)

```bash
# 🐳 Docker Login
docker login

# ☸️ Kubernetes Verification
kubectl get nodes                                  # ✅ verify k8s
kubectl get deployments                            # ✅ verify k8s
kubectl get pods --all-namespaces                  # ✅ verify k8s

# 📦 Run Kubernetes Service
kubectl port-forward svc/homeverse-service 8081:80 # 🚀 to run kubernetes

# 🔐 Get Grafana Password (username: admin)
kubectl get secret grafana -o jsonpath="{.data.admin-password}" | base64 --decode; echo

# 📊 Run Grafana
kubectl port-forward svc/grafana 3001:80           # 📈 to run grafana

# 🧱 Run Docker Container
docker run -p 8081:80 homeverse-app:v1             # 🐳 to run docker containers

