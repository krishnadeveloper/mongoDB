# mongoDB
mongoDB Installation - Process (MacOS)
### Download URL
> https://www.mongodb.com/dr/fastdl.mongodb.org/osx/mongodb-osx-ssl-x86_64-4.0.9.tgz/download
> https://www.mongodb.com/download-center/community (Click on download button by selecting OS from list)

### Installtion Process
 1. Open Terminal
 2. Check mongodb file name like mongodb-osx-ssl-x86_64-4.0.9.tgz
 3. Unzip the file like mongodb-osx-ssl-x86_64-4.0.9.tgz (`tar -zxvf mongodb-osx-ssl-x86_64-4.0.9.tgz`)
 4. Check the directory after unzip and file may be like mongodb-osx-x86_64-4.0.9
 5. Move mongodb-osx-x86_64-4.0.9 directory into local directory (sudo mv mongodb-osx-x86_64-4.0.9 /usr/local/mongodb)
 6. Reach in directory /usr/local/mongodb by using the command `cd /usr/local/mongodb` and check the file `ls -l`
 7. Create some other required directory data, and db inside data directory (`sudo mkdir -p data/db`)
 8. Set permission sudo chown -R `id -un` /data/db (and it may ask Enter your password)
 
 
 ### How to run 
 
 1. Closes terminal window 
 2. Open two termonal window
 3. In one termonal window, run `mongod` (And during start, if you face data/db directory related error or exception then run `mongod --dbpath=/usr/local/mongodb/data/db`)
 4. In 2nd window ], run `mongo` (now mongo shell will be start) 
 
 ### YouTube Video Link
 
 > https://www.youtube.com/watch?reload=9&v=DX15WbKidXY&vl=en
 
