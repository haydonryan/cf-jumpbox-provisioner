cf-jumpbox-provisioner
======================

Provisions an AWS Jumpbox to act as a cloud foundry jump box / work box

Just in case Git isn't present on the AWS image:

```
if [ ! -d ~/workspace ]; then
  mkdir -p ~/workspace
fi
cd ~/workspace
sudo yum -y install git
git clone git@github.com:haydonryan/cf-jumpbox-provisioner.git
```
