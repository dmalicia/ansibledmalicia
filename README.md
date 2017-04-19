# Ansible Deployment LAMP

Simple LAMP on Digital Ocean written on Ansible


### Installing

git clone https://github.com/dmalicia/ansible.git

## Running the tests

 # First run without dynamic inventory
 
 ansible-playbook digitalocean.yml --vault-password-file vault_pass.txt
 
 # Next runs with dynamic inventory
 
 ansible-playbook digitalocean.yml -i digital_ocean.py --vault-password-file vault_pass.txt

Application passwords and services passwords are protected by ansible-vault ( vault-pass.txt )


 # To destroy all machines
 
 ansible-playbook destroydigitalocean.yml --vault-password-file vault_pass.txt

## Built With

* [Ansible]

## Todo

[x] certbot standalone

[] Let's Encrypt 

[] nginx roles

[] high availability on PSQL

[] add new lb instance with keepalive and float ip



## Contributing


## Versioning


## Authors

* **Diego Malicia** - ** - [dmalicia](https://github.com/dmalicia)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments



