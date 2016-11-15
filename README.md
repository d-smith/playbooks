This repo contains a set of playbooks that demonstrate how to install a
simple docker-compose app on a fresh RHEL 7.1 instance. There are 
playbooks to:

* Install docker
* Install docker-compose
* Install certs on the target machine
* Install the docker compose file and the an nginx reverse
roxy config.

Note these need some work to use inventories, groups, plus maybe 
just running each docker service using systemd, etc. So look at this 
as a initial PoC, not as a how to guide.

Unless you dig typing your password over and over you should enable
remote ssh using your key pair, e.g.

<pre>
cd
cat .ssh/id_rsa.pub | ssh user@host 'cat >> .ssh/authorized_keys'
</pre>
