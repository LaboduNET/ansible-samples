# ansible-samples
This repo use ansible files to partially automate VPS deploiements

## Deploy laravel APP

### Server setup
First sample in laravel folder , will deploy a full laravel app on UBUNTU, to use it:
- Ensure you have SSH access to your VPS (Tested on UBUNTU 22.04)
- Ensure your domain has a A Record pointing on your server IP 
- Clone this repo
- Edit the ansible variables (./vars/variables.yml) with the required values
- Run the following command to install all required packages on your VPS: ansible-playbook 1-New_Server_Setup.yml

### Let's Encrypt Configuration
Here the steps depends on several parameters: 
	Do you want a wildcard certicate ou just a domain certificate?
	You DNS provider is sup
If you want a wildcard certificate, you can automate this step if Cerbot support your DNS provider...

TODO:
  - Add folder for shared folders/files (eg: .env, sessions folder...) and create symlinks
  - Update deployements with zero downtime
  - Automate LetEncrypt certificates generation/check/renew
