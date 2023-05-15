# DOS-ILMS STIG for Red Hat Enterprise Linux 7

Ansible Role for DOS ILMS STIG for Red Hat Enterprise Linux 7  

Profile Description:  
This profile contains configuration checks that align to the   
  DOS ILMS STIG for Red Hat Enterprise Linux V1R4.   
    
   In addition to being applicable to RHEL ILMS recognizes this   
  configuration baseline as applicable to the operating system tier of   
  Red Hat technologies that are based off RHEL7, such as:   
  - Red Hat Enterprise Linux Server   
  - Red Hat Enterprise Linux Workstation and Desktop   
  - Red Hat Enterprise Linux for HPC   
  - Red Hat Storage  

The tasks that are used in this role are generated using OpenSCAP.
See the OpenSCAP project for more details on Ansible playbook generation at [https://github.com/OpenSCAP/openscap](https://github.com/OpenSCAP/openscap)

To submit a fix or enhancement for an Ansible task that is failing or missing,
see the ComplianceAsCode project at [https://github.com/ComplianceAsCode/content](https://github.com/ComplianceAsCode/content)

## Requirements

- Ansible version 2.5 or higher

## Role Variables

To customize the role to your liking, check out the [list of variables](vars/main.yml).

## Dependencies

N/A

## Example Playbook

Run `ansible-galaxy install RedHatOfficial.rhel7_stig` to
download and install the role. Then, you can use the following playbook snippet to run the Ansible role:

    - hosts: all
      roles:
         - { role: redhat-ilms }

Next, check the playbook using (on the localhost) the following example:

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml

## License

ILMS-DOS STIG

## Author Information

This Ansible remediation role has been generated from the body of security
policies developed by the ComplianceAsCode project by

Abdoul Alarou

for an updated list of authors and contributors.
Corey Fisher
