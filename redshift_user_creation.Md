Redshift User Creation playbook: 
Main Playbook: https://github.com/philsch/ansible-redshift/blob/master/test/integration/100_test_create_user.yml

Main playbook includes below playbook roles:

Dependencies Validation playbook:
https://github.com/philsch/ansible-redshift/blob/master/test/integration/roles/prepare/tasks/main.yml
Create user tasks after validation:
https://github.com/philsch/ansible-redshift/tree/master/test/integration/roles/test_create_user/tasks


Step1:Execute main.yml, which will run the execute.yml and validate.yml playbooks 
https://github.com/philsch/ansible-redshift/blob/master/test/integration/roles/test_create_user/tasks/main.yml

Step2: Execute execute.yml for Redhshift user creation
https://github.com/philsch/ansible-redshift/blob/master/test/integration/roles/test_create_user/tasks/execute.yml

Step3: Validate if user creation is successful.
https://github.com/philsch/ansible-redshift/blob/master/test/integration/roles/test_create_user/tasks/validate.yml
