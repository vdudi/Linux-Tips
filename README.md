# Linux-Tips
Linux tips


Run a Linux commnad on multiple servers from a single command/loop

for i in {19..22}; do ssh -t 1.2.3.$i "sudo /sbin/service httpd stop" ; done
for i in {19..22}; do ssh -t 1.2.3.$i "sudo /sbin/service httpd start” ; done


