# K8s-Pi-Cluster

https://kubecloud.io/setting-up-a-kubernetes-1-11-raspberry-pi-cluster-using-kubeadm-952bbda329c8

https://blogs.vmware.com/code/2019/06/14/kubernetes-raspberry-pi-cluster/

https://github.com/teamserverless/k8s-on-raspbian/blob/master/GUIDE.md

https://github.com/rancher/k3s/blob/master/README.md

https://sysadmins.co.za/running-k3s-on-the-raspberrypi-4/

https://github.com/teamserverless/k8s-on-raspbian/blob/master/GUIDE.md


kubectl drain <node name> — delete-local-data — force — ignore-daemonsets
kubectl delete node <node name>
Then remove kubeadm completely
kubeadm reset 
# on debian base 
sudo apt-get purge kubeadm kubectl kubelet kubernetes-cni kube* 
#on centos base
sudo yum remove kubeadm kubectl kubelet kubernetes-cni kube*
# on debian base
sudo apt-get autoremove
#on centos base
sudo yum autoremove
 
sudo rm -rf ~/.kube
