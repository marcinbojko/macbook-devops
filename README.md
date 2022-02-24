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

### Install xcode

```bash
ansible-playbook ./macbook-devops.yaml -i ../macbook.lst -e '{"sudo_password": "your_user_password"}'
```

### Variables

#### main playbook

|Variable|Descripton|Default|
|--------|----------|-------|
|install_azure_tools|Install azure-cli|true|
|install_gcloud_tools|Install google-cloud-sdk|true|
|install_oci_tools|Install oci-cli|true|
|install_aws_tools|Install AWS-Cli|true|
|update_homebrew|Should we install homebrew by itself|true|
|update_homebrew_packages|Should we upgrade formulae and casks|true|
|retries_count|how many times retry tasks|2|
|delay_time|how many seconds wait between attempts|3|

#### tasks

|Variable|Descripton|Default|
|--------|----------|-------|
|unpack_folder|where to store downloaded archives| /tmp/macbook|
|bin_path|where to store executable files| /usr/local/bin|

## Content

### Formulae

### Casks

### Tasks

#### `download_files`

Download, unpack and copy executable files from `unpack` section of variables to a folder `bin_path`

example of downloading kubestr file and putting it into `bin_path`

```yaml
unpack:
- url: https://github.com/kastenhq/kubestr/releases/download/v0.4.31/kubestr_0.4.31_MacOS_amd64.tar.gz
  destination: kubestr
  source: kubestr
  destination_file: kubestr.tar.gz
  folder:
```

## ToDO

* add more tools
* add system settings
* add npm
* add external packages not available through homebrew or AppStore

## Known issues

Q: Installation of homebrew casks hangs
A: `sudo_password` variable is not set or set to improper value
