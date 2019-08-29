## MongoDB installation on ubuntu (digital ocean), 

### You can visit on digital ocean link for complete documentation Link : https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-mongodb-on-ubuntu-16-04


## Quck Installation Steps

1. `sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6`
2. `echo "deb [ arch=amd64,arm64 ] http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.4.list`
3. `sudo apt-get update`
4. `sudo apt-get install -y mongodb-org`
5. `sudo systemctl start mongod`
6. `sudo systemctl status mongod`
7. `sudo systemctl enable mongod`

## Securing MongoDB

1. `mongo`
2. `use admin
db.createUser(
  {
    user: "AdminSammy",
    pwd: "AdminSammy'sSecurePassword",
    roles: [ { role: "userAdminAnyDatabase", db: "admin" } ]
  }
)`


