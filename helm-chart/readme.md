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