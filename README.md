Deploy kubernetes on CentOS and Atomic hosts using Ansible
==========================================================

A collection of Ansible roles to deploy a k8s cluster on CentOS and CentOS Atomic hosts.


Usage
-----

```
$ yum install -y ansible
$ ansible-galaxy install -r roles.txt
$ vi hosts
$ ansible-playbook -i hosts deploy-kubernetes.yml
```

At the moment it is assumed there is a `centos` user available on all ndoes to
perform the deployment. This user has to be able to `sudo` without a password.
For CentOS Atomic hosts this is already the case.



Used roles
----------

  * gbraad.docker  
    [Galaxy](https://galaxy.ansible.com/gbraad/docker/), [GitHub](https://github.com/gbraad/ansible-role-docker) / [GitLab](https://gitlab.com/gbraad/ansible-role-docker)
  * gbraad.docker-registry  
    [Galaxy](https://galaxy.ansible.com/gbraad/docker-registry/), [GitHub](https://github.com/gbraad/ansible-role-docker-registry) / [GitLab](https://gitlab.com/gbraad/ansible-role-docker-registry)

  * gbraad.kubernetes-master  
    [Galaxy](https://galaxy.ansible.com/gbraad/kubernetes-master/), [GitHub](https://github.com/gbraad/ansible-role-kubernetes-master) / [GitLab](https://gitlab.com/gbraad/ansible-role-kubernetes-master)
  * gbraad.kubernetes-node  
    [Galaxy](https://galaxy.ansible.com/gbraad/kubernetes-node/), [GitHub](https://github.com/gbraad/ansible-role-kubernetes-node) / [GitLab](https://gitlab.com/gbraad/ansible-role-kubernetes-node)

  * gbraad.kubernetes-client  
    [Galaxy](https://galaxy.ansible.com/gbraad/kubernetes-client/), [GitHub](https://github.com/gbraad/ansible-role-kubernetes-client) / [GitLab](https://gitlab.com/gbraad/ansible-role-kubernetes-client)


Documentation
-------------

Further information about the installation can be found at:

  * [Getting started with containers](https://access.redhat.com/documentation/en/red-hat-enterprise-linux-atomic-host/version-7/getting-started-with-containers/)
  * [Getting started guide](http://www.projectatomic.io/docs/gettingstarted/) at Project Atomic


License
-------

Apache license 2.0


Contributors
------------

  * Gerard Braad
  * Vincent van der Kussen

