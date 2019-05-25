
**If you want to test Docker in your local environment, you need to have Docker installed.**

### Step 1: Clone repo
``` git clone https://github.com/eraldoforgoli/node-docker-test.git ```

### Step 2: Build an image of the Dockerfile located in the root of this repo
```docker build -t node-docker-test . ```  

*the . in the end of the command above represents the path of the Dockerfile, currently . because i am running the docker 
command in the location of git repository*  

### Step 3: Run an instance of this image
``` docker run -d -p 8085:8000 node-docker-test```  

*-d stands for detached mode  
-p stand for port binding, bind the 8085 port in your local machine/server to port 8000 that docker exposes.* 

If you open localhost:8085 in your browser, you should see the app running.

