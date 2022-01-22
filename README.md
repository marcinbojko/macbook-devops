# macbook-devops

Ansible repository for creating DevOps MacBook, based on [https://github.com/marcinbojko/linux_mint](https://github.com/marcinbojko/linux_mint)

## Usage

### Group vars

```yaml
ansible_user: your_user
ansible_port: 22
ansible_connection: ssh
```

```bash
ansible-playbook ./macbook-devops.yaml -i ../macbook.lst -e '{"sudo_password": "your_user_password"}'
```

## ToDO

* add more tools
* add system settings
* add npm
* add external packages not available through homebrew or AppStore
