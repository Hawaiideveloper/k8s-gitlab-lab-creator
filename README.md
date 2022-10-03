# k8s-gitlab-lab-creator

# Work in progress

![Screen Shot 2022-09-29 at 10 48 24 AM](https://user-images.githubusercontent.com/13468708/193063166-a433f50e-a843-4b96-814e-7164ab0ca4cc.png)
#### Use this to stand-up an environment that hosts gitlab 

### Who this is for:
The generalist  
The student / The teacher  
The professional who loves wants to host gitLab locally

### What is Gitlab?
Its a easy to learn and user-friendly devops tool made for creating repositories that can do pipelines and releases on a CI/CD platform

### Why create a Locally hosted gitLab?
Because some people use gitlab at work, and do not want to break the production or try questionable or destructive events on any work environment that could impact their employment; but at the sametime want to test and see the limits of gitlab

### How do you create one?
There are many different ways, but we will be using Kubernetes and Helm.
The method we choose We will be using k8 and helm charts 


#### Prerequisite (Vagrant instance)

- [ ] Create Vagrantfile to stand-up Ubuntu Server 22.04
    - [ ] Ensure the Vagrant file configs at least a 60GB HDD
    - [ ] Has a bridged network interface


### Stand-up a Ubuntu Server 18.04 using vagrant

Prerequisites
Working Vagrant setup
8 Gig + RAM workstation as the Vms use 3 vCPUS and 4+ GB RAM
For MAC/Linux Users
Latest version of Virtualbox for Mac/Linux can cause issues because you have to create/edit the /etc/vbox/networks.conf file and add:

* 0.0.0.0/0 ::/0
or run below commands

sudo mkdir -p /etc/vbox/
echo "* 0.0.0.0/0 ::/0" | sudo tee -a /etc/vbox/networks.conf
So that the host only networks can be in any range, not just 192.168.56.0/21 as described here: https://discuss.hashicorp.com/t/vagrant-2-2-18-osx-11-6-cannot-create-private-network/30984/23




### Install [Kubernetes Cluster](https://alta3.com/blog/singlevmk8s)
### Deploy [Gitlab](https://docs.gitlab.com/charts/installation/) on it


