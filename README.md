# Simple implementation of CIS RHEL 8  chapter 1.7 Warning Banners with the help of Ansible playbooks. 

Playbooks add a secure_banners role which handles files.  
As an example playbook workstation.yml applies this role and accompanying tasks to hosts in [workstation] group.  
Assumtions taken:  
- All hosts are already setup with ansible and ssh keys 
- We already have passwordless sudo on hosts 
- Banners should be the same on all [workstation] members
