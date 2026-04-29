K8s Aduit to scan the cluster for any kind of issues

wget https://github.com/Shopify/kubeaudit/releases/download/v0.22.2/kubeaudit_0.22.2_linux_amd64.tar.gz
tar -xvzf kubeaudit_0.22.2_linux_amd64.tar.gz
mv kubeaudit /usr/local/bin
kubeaudit all


generate self signed cert and key then
kubectl create secret tls devops-aul --cert=/C/Users/user/Desktop/Aul/devops/devops-assignment/tls.crt --key=/C/Users/user/Desktop/Aul/devops/devops-assignment/tls.key -n devops
