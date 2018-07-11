This assumes that ansible is installed and you are running on a Linux OS.

First pull down ansible roles in the `roles/` directory
```
ansible-galaxy install -r roles/requirements.yml -p roles
```

Run the playbook specifying your AWS access and secret key
```
ansible-playbook -i inventory/dev/hosts --extra-vars "aws_access_key_id=YOUR_ACCESS_KEY_ID aws_secret_access_key=YOUR_SECRET_ACCESS_KEY"
```
