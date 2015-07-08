cf-jumpbox-provisioner
======================

Provisions an AWS Jumpbox (either ubuntu or AWS Linux centos) to act as a cloud foundry jump box / work box

Git isn't present on the AWS Linux AMI (HVM) image:

```
if [ ! -d ~/workspace ]; then
  mkdir -p ~/workspace
fi
cd ~/workspace
sudo yum -y install git
git clone http://github.com/haydonryan/cf-jumpbox-provisioner.git
cd cf-jumpbox-provisioner
```

Git isn't present on the AWS Ubuntu 14.xx image:
```
if [ ! -d ~/workspace ]; then
  mkdir -p ~/workspace
fi
cd ~/workspace
sudo apt-get -y install git
git clone http://github.com/haydonryan/cf-jumpbox-provisioner.git
cd cf-jumpbox-provisioner
```
