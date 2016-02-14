# NGINX Mainline Playbook

This playbook installs and sets up NGINX Mainline on remote servers.

## Deployment

Before running the below commands, make sure the correct user account is selected in ./server.yml

For staging / lab deployment:

```shell
~/g/ansible-nginx ❯❯❯ ansible-playbook --become --become-method=su --become-user=root --ask-become-pass -i staging deploy.yml
```

For production / live deployment:

```shell
~/g/ansible-nginx ❯❯❯ ansible-playbook --become --become-method=su --become-user=root --ask-become-pass -i production deploy.yml
```
