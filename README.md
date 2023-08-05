# Installing AWS CLI

## Install cli

```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

unzip awscliv2.zip

sudo ./aws/install

# verify aws installation
aws --version
```

## Enable auto complete

### Modify .zshrc file

Add the code below to the end of the .zshrc file.

```bash
# aws autoload
autoload bashcompinit && bash compinit

autoload -Uz compinit && compinit
```

### Run this command in terminal

```bash
complete -C '/usr/local/bin/aws_completer' aws
```
