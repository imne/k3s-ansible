
<!-- It's a good idea to check this post first for general troubleshooting https://github.com/techno-tim/k3s-ansible/discussions/19   -->

<!--- Provide a general summary of the issue in the Title above -->

## Expected Behavior

<!--- Tell us what should happen -->

## Current Behavior
<!--- Tell us what happens instead of the expected behavior -->

## Steps to Reproduce

<!--- reproduce this bug. Include code to reproduce, if relevant -->

1.
2.
3.
4.

## Context (variables)
<!--- please include which OS, along with the variables used when running the playbook -->

Operating system:

Hardware:

### Variables Used

`all.yml`

```yml
k3s_version: ""
ansible_user: NA
systemd_dir: ""

cert_manager_notify_email: ""
cert_manager_version: ""
cert_manager_cloudflare_api_token: ""

flannel_iface: ""

apiserver_endpoint: ""

k3s_token: "NA"

extra_server_args: ""
extra_agent_args: ""

kube_vip_tag_version: ""

metal_lb_speaker_tag_version: ""
metal_lb_controller_tag_version: ""

metal_lb_ip_range: ""

externaldns_pihole_server: ""
externaldns_password: ""

longhorn_version: "v1.6.2"
rancher_url: "rancher.kwamlng.dev"
rancher_adminPassword: ""

```

### Hosts

`host.ini`

```ini
[master]
IP.ADDRESS.ONE
IP.ADDRESS.TWO
IP.ADDRESS.THREE

[node]
IP.ADDRESS.FOUR
IP.ADDRESS.FIVE

[k3s_cluster:children]
master
node
```

## Possible Solution
<!--- Not obligatory, but suggest a fix/reason for the bug, -->

- [ ] I've checked the [General Troubleshooting Guide](https://github.com/techno-tim/k3s-ansible/discussions/20)
