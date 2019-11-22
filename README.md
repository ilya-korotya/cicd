# Setup Jenkins
Ansible script to help install Jenkins on the target server

### How it use?

1. Install `ansible` and `ansible-playbook`;
2. Run command (By default will use SSL certificate):
    ```
      ansible-playbook -i <YOUR_IP_ADDRESS>, jenkins.yml
    ```

### How configuration Jenkins?
1. You can use `roles/jenkins/defaults/main.yml` for configuration `defaults path to Jenkins`, `SSL/TLS certificates` and `Jenkins HTTP/HTTPS ports`
       
    For example. If you want use yourslef own `SSL/TLS certificates` set variables:
    ```
    jenkins_user_ssl_private_key: ~/.ssh/My_private_key
    jenkins_user_ssl_certificate: ~/.ssh/My_ssl_certificate
    ```
2. For other settings you mast use `roles/jenkins/files/jenkins.env` file.

### What systems can I use?
This `ansible` script has been tested on `CentOS 7` and `Ubuntu 16.04-18.04`. But you can use `Debian` and `RedHat` family systems.
