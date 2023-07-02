# ansible-samples
This repo use ansible files to automate VPS deploiements

First sample, deploy a full laravel app, to use it:
- Clone this repo
- Edit the ansible variables with the required values
- Run the following command: ansible-playbook deploy.yml

TODO:
  - Add folder for shared folders/files (eg: .env, sessions folder...) and create symlinks
  - Update deployements with zero downtime
  - Automate LetEncrypt certificates generation/check/renew
