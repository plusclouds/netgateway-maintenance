# plusclouds.automation,netgateway.ntp.install

This role will install and set up ntp for target host if it is not installed yet. You can also update your already installed and created ntp, this role replace /etc/ntp.conf file with our template in every run.

## Role Variables

---

| Variable      | Required | Example                          | Comments                                                                             |
| ------------- | -------- | -------------------------------- | ------------------------------------------------------------------------------------ |
| user_token:   | yes      |                                  | Your token                                                                           |
| leo_url       | yes      | http://10.100.0.114              | Url address of target dc                                                             |
| pools         | yes      | [0.pool.ntp.org, 1.pool.ntp.org] | Use comma between each pool! This variable is an array, don't forget square brackets |
| timezone      | yes      | "Europe/Istanbul"                | Timezone                                                                             |


## Example Playbook

```YAML
- name: Install NTP to Netgateway
  hosts: netgateway
  become: false
  gather_facts: false
  roles:
    -  role: plusclouds.environment.information
    -  role: plusclouds.netgateway.configs.get
    -  role: plusclouds.netgateway.ntp.install
  vars:
    - user_token: ""
    - leo_url: http://10.100.0.114
    - pools: [0.pool.ntp.org, 1.pool.ntp.org, 2.pool.ntp.org]
    - timezone: "Europe/Istanbul"
  environment:
    ANSIBLE_HOST_KEY_CHECKING: false

```

## Author Information

Yigithan Saglam - yigithan.saglam@plusclouds.com