# test-task

## Dependencies
First install dependecies 
```
ansible-galaxy install -r requirements.yaml
```

## Run
Before run, provide neccessary information about your hosts in `inventory` folder:  
1. Create file at `inventory/host_vars` with prefered name at describe information about your host
2. Add your host in specific group at `inventory/hosts` file

After run playbook
```
ansible-playbook -u ubuntu -i inventory prepare_server.yaml --diff --private-key=/path/to/key.pem --ask-vault-pass
```
Vault pass is `test`
