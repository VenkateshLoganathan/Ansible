jenkins
=========

Install Jenkins continuous integration package on RHEL/CentOS and Ubuntu servers.

Requirements
------------

CentOS server - 6 and 7

Role Variables
--------------

baseurl: "http://pkg.jenkins.io/redhat"
gpgkey: "http://pkg.jenkins-ci.org/redhat/jenkins-ci.org.key"


Dependencies
------------

Example Playbook
----------------

---
- hosts: jenkins
  become: yes
  become_user: root
  vars:
    baseurl: "{{ baseurl }}" 
    gpgkey: "{{ gpgkey }}" 

  roles:
    - jenkins


License
-------

BSD

Author Information
------------------

Venkatesh.L - DevOps Engineer in CD CloudEnablers pvt ltd.
