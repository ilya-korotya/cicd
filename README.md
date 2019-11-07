# Setup CI/CD via ansible. terraform and Jenkins

### How to use it?

1. Add ssl certificate for SSH connect to `~/.ssh/`;
2. Run ansible palybook:
```
ansible-playbook jenkins.yml  -i 52.57.142.122,
```
