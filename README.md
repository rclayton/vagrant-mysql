Vagrant MySQL-box
=================

This is a no frills MySQL box.  I use it for development, particularly when I'm hosting the server runtime on my local machine (whether it be Node, Python or Golang).

### MySQL Info

**Username**: root

**Password**: password

You can change this by modifying the `playbook.yml`.  If you do change the password, remember to update the `my.cnf` file as well.

The test database is also removed, and IPTables is turned off.  I'm using this in a private network on my local box and don't need much security.
