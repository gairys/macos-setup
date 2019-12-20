# macos-setup
Setting up my new macbooks with ansible and homebrew.
- - - 

I enjoy playing with Ansible and decided to apply what I've learned to setting up my Mac products somewhat consistently. I had a fairly linear layout for my last setup, but decided to go with a more traditional Ansible playbook layout.

### Giving thanks first

First, I'd like to thank the many people from GitHub who I referenced while setting up this repo for myself.

https://github.com/geerlingguy/mac-dev-playbook

https://github.com/geerlingguy/ansible-role-homebrew

https://github.com/daemonza/setupmac

https://github.com/feffi/ansible-macos-computername

https://github.com/adamchainz/mac-ansible

https://daemonza.github.io/2017/03/06/using-ansible-to-automate-my-macbook-setup/

https://adamj.eu/tech/2019/03/20/how-i-provision-my-macbook-with-ansible/

https://medium.com/tensult/setting-up-a-mac-using-ansible-3dcf63c1d324

https://code-maven.com/enable-ansible-passwordless-sudo

### Fixing the first of many errros

Following these sites, I started to get a depreciation warning when the playbook was running:

```bash
[DEPRECATION WARNING]: Invoking "homebrew" only once while using a loop via 
squash_actions is deprecated. Instead of using a loop to supply multiple items 
and specifying `name: {{ item }}`, please use `name: u'{{ brew_packages }}'` 
and remove the loop. This feature will be removed in version 2.11. Deprecation 
warnings can be disabled by setting deprecation_warnings=False in ansible.cfg.
```

I found the solution on the following page, using Google Translate to get what I needed.

https://translate.google.com/translate?hl=en&sl=ja&u=https://dev.classmethod.jp/etc/mrmo-first-mac-setup-ansible/&prev=search

https://dev.classmethod.jp/etc/mrmo-first-mac-setup-ansible/

