# PostgreBackup-Using-Kubernetes-Cronjob
## DevOps Project

### Project Requirements

+ Shell Scripting
+ Vagrant
+ Terraform
+ Helm Chart
+ Docker
+ Kubernetes
+ Jenkins
+ Ubuntu 21.04
+ Redis
+ PostgreSQL

** _NOTE : We will create 1 master and 2 worker nodes using Vagrant. **

** _NOTE : We will use Terraform to create infrastructure for local clusters to run on the cloud. **

`vagrant up` --> all Clusters are started.<br>
`vagrant status`--> check the status of Clusters<br> 
`vagrant ssh "node name"`-->node by ssh.<br>

![vagrant](https://user-images.githubusercontent.com/42733209/169891496-9482b253-401b-4c9e-9487-96e804f5e1da.png)


## Jenkins Installation 
`sudo apt-get update`<br>
`sudo apt-get install openjdk-8-jdk`<br>
`wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -`<br>
`sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'`<br>
`sudo apt-get update`<br>
`sudo apt-get install jenkins`<br>
https://localhost:8080

![1_fiOou8ZYaZe-Ka8NUyovMw](https://user-images.githubusercontent.com/42733209/169891698-0469019b-d39f-4775-acdc-12db2a33d819.png)



                                LOCAL KUBERNETES CLUSTER  -- Break 
                               
# In summary: 
###### 1- Setting up 1 master and 2 worker nodes using Vagrant
###### 2- Installing kubernetes inside these VMs
###### 3- Installing Jenkins on the master
###### 4- Creating a postgre pod on Node1
###### 5- Creating a redis pod on Node2
###### 6- Yaml files should be prepared for these installations in the master.
###### 7- Kubernetes cronjob will be prepared for Postgre backup in master. A sh will be written about it.
###### 8- We will make Helm after the kubernetes installation and manage all the deployment processes through this chart.
###### 9- Establishing the infrastructure that can work on the cloud with Terraform





