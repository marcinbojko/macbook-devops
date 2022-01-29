# macbook-devops

Ansible repository for creating DevOps MacBook, based on [https://github.com/marcinbojko/linux_mint](https://github.com/marcinbojko/linux_mint)

## Usage

### Enable `ssh` aka `remote access`

![ssh](./images/ssh.png)

### Group vars

```yaml
ansible_user: your_user
ansible_port: 22
ansible_connection: ssh
```

```bash
ansible-playbook ./macbook-devops.yaml -i ../macbook.lst -e '{"sudo_password": "your_user_password"}'
```

### Variables

|Variable|Descripton|Default|
|--------|----------|-------|
|install_azure_tools|Install azure-cli|true|
|install_gcloud_tools|Install google-cloud-sdk|true|
|install_oci_tools|Install oci-cli|true|

## Content

### Formulae

### Casks

## ToDO

* add more tools
* add system settings
* add npm
* add external packages not available through homebrew or AppStore

## Known issues

Q: Installation of homebrew casks hangs
A: `sudo_password` variable is not set or set to improper value
