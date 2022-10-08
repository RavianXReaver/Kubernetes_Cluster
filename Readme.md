# **Microk8s HA Cluster**


Under construction....

Notes:

To access and remotely connect to the kubectl in master node from localhost use the below command.

scp -r vagrant@[IP_address]:/home/vagrant/.kube/config ~/.kube/config
Then Change the server address in ~/.kube/config

**POST CONFIGURATION**

Step 1: Create the kube config file in the master node 
``ssh vagrant@[MasterNode_IP_address] microk8s config > ~/.kube/config``
Step 2: Copy the Kube config file to the local server 
``scp -r vagrant@[MasterNode_IP_address]:/home/vagrant/.kube/config ~/.kube/config``