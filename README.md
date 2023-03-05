# Ansible_Automations
 The automation files use a become password encrypted vault which is places in the var file named pass.yaml. 
 For security reasons the file is not included in the repo. In-order for the playbooks to work as expected, do the below steps:
 <ol>
 <li>Create a file name pass.yaml.</li>
 <li>Add the line: 'ansible_become_pass: your_become_password'</li>
 <li>Run the ansible vault module to encrypt the become password in the file: 'ansible-vault encrypt pass.yaml'</li>
 <li>Enter your desired vault password</li>
 <li>While running the playbook add the --ask-vault-pass flag. Ex: 'ansible-playbook playbook.yaml --ask-vault-pass'</li>
 </ol>
 
