# test-infra
Nephio project's test infrastructure configuration &amp; tools for metal3 infra is maintained in this repository.

**Note**: Issues should be opened in the [sig-release](https://github.com/nephio-project/sig-release)
repository.

### Modified Upstream Project
Nephio Project Official [Here](https://github.com/nephio-project/test-infra.git)

### Same project configured for running on AWS EC2
Nephio AWS [Here](https://github.com/vitu1234/nephio-test-infra-aws.git) 

### Same project configured for running on OpenStack
Nephio OpenStack [Here](https://github.com/vitu1234/nephio-test-infra-openstack.git) 

### Run the following Galaxy commands
ansible-galaxy collection install ansible.posix
ansible-galaxy collection install community.general
ansible-galaxy collection install openstack.cloud

### run the following commands
cd nephio/test-infra-aws/e2e/provision/
pip install -r requirements.txt
export PATH="$PATH:/home/ubuntu/.local/bin"
source ~/.bashrc
ansible-galaxy install -r galaxy-requirements.yml
./install_sandbox.sh