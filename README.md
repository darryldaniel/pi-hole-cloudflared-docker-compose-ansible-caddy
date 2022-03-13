# Example Docker Compose and Ansible configuration for running Pi-Hole, Cloudflared, and Caddy

Example configuration for using Pi-Hole, Cloudflared, Docker Compose, Ansible, and Caddy to over-engineer your home network for privacy and security.

## Details

See [How I re-over-engineered my home network for privacy and security](https://ben.balter.com/2021/09/01/how-i-re-over-engineered-my-home-network/) (and [How I over-engineered my home network for privacy and security](https://ben.balter.com/2020/12/04/over-engineered-home-network-for-privacy-and-security/)).

## Usage

1. Encrypt secrets with `ansible-vault encrypt secrets.enc`
2. Run the playbook with `ansible-playbook -i hosts.yml -e @secrets.enc --ask-vault-pass playbook.yml`
