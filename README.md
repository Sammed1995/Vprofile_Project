# Vprofile_Project
Multi-vm project

VM SETUP
1.	Clone source code.
2.	Cd into the repository.
3.	Switch to the main branch.
4.	cd into vagrant/Manual_provisioning
Bring up vm’s
$ vagrant up
NOTE: Bringing up all the vm’s may take a long time based on various factors. If vm setup stops in the middle run “vagrant up” command again.
INFO: All the vm’s hostname and /etc/hosts file entries will be automatically updated

Setup should be done in below mentioned order
1.	MySQL (Database SVC)
2.	Memcache (DB Caching SVC)
3.	RabbitMQ (Broker/Queue SVC)
4.	Tomcat	(Application SVC)
5.	Nginx	(Web SVC)



