# Raspberry Pi Media Center

The purpose of this repository is to provide an ansible playbook for managing multiple raspberry pi media center installations. Playbook runs on Raspberry Pi with default LibreELEC installation and performs these tasks:

 * Use public/private key based SSH authentication and disable password authentication for root
 * Setup correct timeservers
 * Setup TV using vdr backend
 * ...

# Precondition

 * ansible-galaxy install cmprescott.xml

# Usage LibreELEC

 * setup the raspberry pi with LibreELEC
 * create file files/authorized_keys.myuser.pub and add your public SSH key to this file
 * when running playbook the first time, type "ansible-playbook setup-libreelec.yml --ask-pass"
 * after first run, you can omit --ask-pass
