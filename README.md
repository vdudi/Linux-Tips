# Linux-Tips
Linux tips


Run a Linux commnad on multiple servers from a single command/loop

  for i in {19..22}; do ssh -t 1.2.3.$i "sudo /sbin/service httpd stop" ; done

  for i in {19..22}; do ssh -t 1.2.3.$i "sudo /sbin/service httpd start” ; done

Copy SSH keys to a Linux server so you don't have to type password.

  ssh-copy-id IP

Delete similar name folders - list & delete

  sudo find  /home/ -name "2014*" -ls
  sudo find /home/ -name "2014*" -exec rm -rf {} \;
