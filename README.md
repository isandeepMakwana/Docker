
> What is docker

A platform for biulding running and shipping application and consistently build,run and ship application

> Container

- An isolated environment for running an application

- Allow running multiple app in isolation
Are lightweight
Use os of the host
start queickly
need less hardware resource

`let's geate project and dockerzie`

create Folder :
```bash
 mkdir hello-docker
```

> Inside of this folder and create one file
 ```javascript
  -->file_name.js<--
  console.log("hello World");
  ```


> Instruction To Deploy Application

- start with os
- install node
- copy app files
- run node file-name.js (main_file)

go-back to hello-docker folder and create one file

 <mark>Dockerfile<mark>

	-->dockerfile<---
from ---
   we need a base image so we can us linux image and than install node or use directly node image

 ```docker
FROM   node:alpine
                     <!-- you can specify the the version of linux distribution -->

COPY    .    /app
                <!-- in this image create file docker from
                current directory and copy all the on app system-->
                <!-- copy all the files from current folde -->
                <!-- path directry to (/app directry) -->

CMD   node   /app