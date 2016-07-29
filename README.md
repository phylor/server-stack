# Server Stack

This is an opinionated provisioning script which installs basic services for external facing servers.

## Installed Components

- Docker
- HTTPS Proxy
- Monitoring
- Letsencrypt

## Provisioning

To provision one or multiple servers, do the following:

- `git clone git@github.com:phylor/server-stack.git`
- `cd server-stack`
- Create an inventory file `inventories/myinventory`. Note that your servers need to include a variable called `email` specifying the administrator's email address, e.g.:

     ```c
     [servers]
     1.1.1.1    ansible_user=root email=admin@example.com
     ```


- `ansible-playbook -i inventories/myinventory preparation.yml`
- `ansible-playbook -i inventories/myinventory server.yml`

## Recommended Monitoring Dashboards

- https://grafana.net/dashboards/193
- https://grafana.net/dashboards/22
