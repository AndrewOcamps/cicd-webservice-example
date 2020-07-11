# cicd-webservice-example
This project is used to complement the tutorial published on the following page: https://medium.com/@blog.ocampoge/ci-cd-automatiza-tus-despliegues-con-gitlab-y-ansible-79876bec9c18

Vagrant configuration file to install the CI CD Gitlab lab environment

Before you start, you must have the following components installed on your workstation

* Vagrant:https://www.vagrantup.com/downloads.html
* Virtualbox: https://www.virtualbox.org/wiki/Downloads

Inside the infrastructure directory is the Vagrantfile file, used to deploy servers

### Step 1:
```
cd infrastructure
vagrant up
```

### Step 2:
In a terminal access the configured virtual machines
```
(CICD GitLab Server)
ssh vagrant@192.168.33.20
pass: vagrant
```

```
(Web Development Server)
ssh vagrant@192.168.33.21
pass: vagrant
```

```
(QA Web Server)
ssh vagrant@192.168.33.22
pass: vagrant
```

```
(Web Production Server)
ssh vagrant@192.168.33.23
pass: vagrant
```

```
(Gitlab Runner + Ansible Server)
ssh vagrant@192.168.33.24
pass: vagrant
```

### Step 3:
In the browser access http://192.168.33.20/
Set GitLab admin password

Continue at the following link: https://medium.com/@blog.ocampoge/ci-cd-automatiza-tus-despliegues-con-gitlab-y-ansible-79876bec9c18
