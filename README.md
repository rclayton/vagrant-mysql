Vagrant MySQL-box
=================

This is a no frills MySQL box.  I use it for development, particularly when I'm hosting the server runtime on my local machine (whether it be Node, Python or Golang).

#### Update July 19, 2014

I've updated this install script to use the latest version of MySQL.  Legally, you need to go accept the Oracle "Terms of Service" for MySQL here:  http://dev.mysql.com/downloads/file.php?id=450542.  I'm serious about this.  I have no right to distribute MySQL (it's Oracle product).  Please note that you have been warned!

Assuming you have done accepted the terms of service, these scripts will automate the install.

### MySQL Info

**Username**: root

**Password**: password

You can change this by modifying the `root_db_password` variable in `playbook.yml`.  I've changed the playbook to ensure the `.my.cnf` also uses this value.

The test database is also removed, and IPTables is turned off.  I'm using this in a private network on my local box and don't need much security.
