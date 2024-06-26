
**Ansible deployment**

To run the ansible code, you need to make sure you have ansible-playbook installed on your system
`python3 -m install pip install ansible-core`

This should do the work to install ansible.

There is hosts.ini file, which is basically an inventory file (currently empty with ip or domain name) but need to populate the file.
There is sites.yml file, to tell which tasks to run

To run the ansible, you need to do
`ansible-playbook -i hosts.ini sites.yml`


**Jenkinsfile**

Just copy the content of Jenkinsfile inside CICD/jenkins folder in the same repo, root folder of python based lambda code. Once you have saved there, you should be able to run the Jenkins job using this jenkinsfile to lint, unit test, build as well as run security scan and deploy the lambda code.
