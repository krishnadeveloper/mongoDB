# mongoDB
mongoDB Installation - Process (MacOS)
### Download URL
> https://www.mongodb.com/dr/fastdl.mongodb.org/osx/mongodb-osx-ssl-x86_64-4.0.9.tgz/download
> https://www.mongodb.com/download-center/community (Click on download button by selecting OS from list)

### Installtion Process
 1. Open Terminal
 2. Check mongodb file name like mongodb-osx-ssl-x86_64-4.0.9.tgz
 3. Unzip the file like mongodb-osx-ssl-x86_64-4.0.9.tgz (`tar xzf mongodb-osx-ssl-x86_64-4.0.9.tgz`)
 4. Check the directory after unzip and file may be like mongodb-osx-x86_64-4.0.9
 5. Move mongodb-osx-x86_64-4.0.9 directory into local directory (sudo mv mongodb-osx-x86_64-4.0.9 /usr/local/mongodb)
 6. Reach in directory /usr/local/mongodb by using the command `cd /usr/local/mongodb` and check the file `ls -l`
 7. Create some other required directory data, and db inside data directory (`sudo mkdir -p data/db`)
 
