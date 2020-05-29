# Instalacion Docker
<pre>
sudo apt remove docker docker-engine docker.io
sudo apt install apt-transport-https ca-certificates curl software-properties-common gnupg
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt update
sudo apt install docker-ce
sudo usermod -aG docker $USER
</pre>
# Instalacion Docker
<pre>
sudo apt install docker-compose
</pre>
# Instalacion Minikube
<pre>
sudo apt-get update
sudo apt-get install apt-transport-https
sudo apt-get upgrade
#sudo apt install virtualbox virtualbox-ext-pack
wget https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
chmod +x minikube-linux-amd64
sudo mv minikube-linux-amd64 /usr/local/bin/minikube
</pre>
# Instalacion Kubectl
<pre>
curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
chmod +x ./kubectl
sudo mv ./kubectl /usr/local/bin/kubectl
</pre>
# Arrancar Minikube
<pre>
minikube start
</pre>
# Comprobación de versiones
<pre>
minikube version
kubectl version -o json 
</pre>
# Instalacion Helm
<pre>
sudo snap install helm --classic
</pre>
