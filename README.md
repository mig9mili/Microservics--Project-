# Microservics--Project-
README file for running Emart App using Vagrant and Docker

Introduction:
Emart App is an e-commerce web application that can be run using Vagrant and Docker. This README file will guide you through the steps to download and run the application on your local machine.

Prerequisites:
- Vagrant installed on your local machine
- Docker installed on your local machine

Steps:

1. Download the microapp folder from the given link.

2. In the command window, navigate to the directory where the microapp folder is downloaded and follow the steps below:

    a. Run the command: `vagrant up` - This will start the virtual machine.
   
    b. Run the command: `vagrant ssh` - This will connect you to the virtual machine.
    
    
    c. Run the command: `sudo -i` - This will log you in as the root user.
    
    
    d. Clone the source code of Emart App by running the command: `git clone https://github.com/devopshydclub/emartapp.git
    
    
    e. Run the command: `ls` - This will show you the emartapp directory.
    
    
    f. Enter into the emartapp directory by running the command: `cd emartapp/`
    

3. Next step is to run the container from the docker-compose file. Follow the steps below:


    a. Run the command: `docker-compose up -d` - This will start the containers required to run the application. It may take some time to download and build the required images.
    
    
    b. Run the command: `docker ps` - This will show you the running containers. Check if the nginx container is running.
    
    
    c. Get the IP address by running the command: `ip addr show` - Copy the IP address.
    
    
 
    d. Open your browser and enter the URL: `http://<copied_ip_address>:80` - This will show you the Emart App running in your browser.
    

4. For clean up, run the command: `docker-compose down` - This will stop and remove the containers created.


Conclusion:
Following the above steps, you can easily download and run the Emart App using Vagrant and Docker on your local machine.
