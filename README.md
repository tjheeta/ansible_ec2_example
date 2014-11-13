    sudo apt-get install ansible
    sudo apt-get install boto

    $ cat ~/.boto 
    [Credentials]
    aws_access_key_id = YOUR_ACCESS_KEY
    aws_secret_access_key = YOUR_SECRET_KEY

    ansible-playbook  --private-key=~thekey.pem -i inventory ec2_tasks/create.yml
    ansible-playbook  -i inventory ec2_tasks/delete.yml
