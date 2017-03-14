# OS_create-users

## Install Terraform and Packer on Ubuntu 16.04 LTS
```bash
sudo unlink /usr/bin/terraform                                                                                                                                                                                                       
sudo unlink /usr/bin/packer
mkdir ~/{terraform_0.8.6,packer_0.12.3}


rm /usr/bin/{terraform,packer}

cd ~/terraform_0.8.6 && curl -O https://releases.hashicorp.com/terraform/0.8.6/terraform_0.8.6_linux_amd64.zip
cd ~/packer_0.12.3 && curl -O https://releases.hashicorp.com/packer/0.12.3/packer_0.12.3_linux_amd64.zip
cd ~/terraform_0.8.6 && unzip terraform_0.8.6_linux_amd64.zip && sudo ln -s ~/terraform_0.8.6/terraform /usr/bin/terraform
cd ~/packer_0.12.3 && unzip packer_0.12.3_linux_amd64.zip && sudo ln -s ~/packer_0.12.3/packer /usr/bin/packer
```