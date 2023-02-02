
# MINIKUBE-TO-CREATE-CLUSTER


### Step 1 : Create an AWS EC2 instance with Ubuntu 22.
* Create an EC2 instance with Ubuntu 22.04 (the latest for the moment) operating system.

* Instance Size: t2.large with 2 CPUs, 32 GB Storage

### Step 2 : Install Docker.

### Step 3 : Install Kubectl :
```bash
 curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -

 sudo touch /etc/apt/sources.list.d/kubernetes.list

 echo "deb http://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee -a /etc/apt/sources.list.d/kubernetes.list

 sudo apt-get update

 sudo apt-get install -y kubectl
```
### Step 4: Install Minikube :
```bash
  curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
```
```bash
  sudo install minikube-linux-amd64 /usr/local/bin/minikube
```
### Now start the minikube with following command :
```bash
 minikube start
```
### If you got a error enter the below command to start minikube :
```bash
 minikube start --force
```

