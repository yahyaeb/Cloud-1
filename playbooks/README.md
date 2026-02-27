docker run --rm -it   -v /home/yel-bouk/Documents/Cursus/Cloud-1/playbooks:/work -w /work   -v /home/yel-bouk/.ssh:/root/.ssh:ro   willhallonline/ansible:latest   sh -lc 'ansible-galaxy role install geerlingguy.docker -p /work/roles && ansible-playbook -i inventory.ini clone_file.yaml -K'

