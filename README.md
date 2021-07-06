# Project Title

Collection of Ansible roles for deployment of Kadalu operator

## Description

Despite being easy, manual deployment always have the risk of missing vital steps or even implementing it in the wrong order.
These roles should allow end-users to implement Kadalu in a straigtforward way.

Any PRs are always welcome!

## Getting Started

### Dependencies

Ansible v2.9
Direct connectivity to:
  - github.com (kadalu.io)
  - pypi.org (openshift/kubernetes pip modules)

### Installing

# Clone this repo
git clone git@github.com:kadalu/kadalu-ansible.git

### Executing program

```
# Adjust your inventory
vim inventories/inventory

# Adjust your group and/or host variables
vim  group_vars/kubernetes_nodes

mkdir host_vars/kube1.localdomain
vim host_vars/kube1.localdomain

# Adjust the roles you need in the roles section of the sample.yml
cp -a sample.yml mydeployment.yml
vim mydeployment.yml

# Run ansible in dry-run mode
ansible-playbook -i inventories/inventory mydeployment.yml --check

```

## Help

Ensure that you have direct access as per the dependency section.
If direct access is not possible, you have to adjust the role,
so you can obtain the relevant binaries/pip modules.

## Authors

```
# Strahil Nikolov 
Slack:
---> https://app.slack.com/client/TGX174QDQ/CGWT9RFFD/user_profile/U0278G3CD5W
---> https://app.slack.com/client/TGX174QDQ/learning-slack/user_profile/U026THB01SB
E-mail:
---> hunter86_bg@yahoo.com
---> strahil.nikolov@gmail.com
```

## License

<To be discussed>
