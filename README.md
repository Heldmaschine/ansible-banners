# Simple implementation of CIS RHEL 8  chapter 1.7 Warning Banners with the help of Ansible playbooks. 

Playbookks are split per subchapter, as indicated by playbook `name` attribute.
Use `--tags audit` to run only audit and `--tags remediation` to run only remediation steps.
For MOTD chapter additional `--tags remediation_alt` included to remove the file, as adviced by chapter.
Assumptions taken:  
- All hosts are already setup with ansible and ssh keys
- All hosts are in [workstation] ansible group
- We already have passwordless sudo on hosts 
- Template files are already within site policy (currently example content for chapters)
