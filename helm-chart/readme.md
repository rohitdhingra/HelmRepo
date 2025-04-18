1. helm create hello-world-helm-chart
2. minikube addons enable ingress
3. minikube tunnel
2. helm install hello-world-app ./hello-world-helm-chart
3. helm install hello-world-app ./hello-world-helm-chart --set ingress.enabled=true
4. sudo nano /etc/hosts
   127.0.0.1 springboot.local

5. sudo dscacheutil -flushcache
   sudo killall -HUP mDNSResponder
6. ping springboot.local
7. Open browser and run http://springboot.local/
8. helm uninstall hello-world-app