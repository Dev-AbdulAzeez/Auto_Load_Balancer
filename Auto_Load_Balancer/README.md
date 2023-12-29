# **_Automating Load Balancer Configuration with Shell Scripting_**

+ **Introduction**

Automating load balancer configuration using shell scripting and CI/CD on Jenkins offers significant benefits. This documentation outlines a project that demonstrates how to automate load balancer setup and maintenance, reducing manual effort and enhancing efficiency.

+ **Project Overview**

+ The project focuses on automating the deployment and configuration of webservers using the following steps:

+ Load Balancer Setup: Set up a load balancer using Nginx to distribute traffic across multiple webservers efficiently.

+ Manual Configuration: Initially, perform load balancer setup manually to establish a baseline understanding.

+ Automation with Shell Scripting: Create a shell script to automate load balancer configuration, encapsulating necessary commands and configurations.

+ CI/CD Integration: Integrate the shell script into a CI/CD pipeline on Jenkins for automatic execution upon code or configuration changes.

Freestyle Job Execution: Create a freestyle job in Jenkins to trigger the execution of the shell script, either scheduled or manually.

## **Deploying and Configuring the Webservers**

Follow the steps below to run the script:

+ Step 1: Provision an EC2 instance running bunt 20.04. You can refer to the course Implementing load balancer with Nginx for a refresher

+ Step 2: Open port 8000 to allow traffic from anyhere using the security group. Again refer to the course mentioned above in step one for a refresher.

+ Step 3: Connect to the webserver via the terminal using SSH clint

+ Step 4: Open a file, paste the script above and close the file using the command below:

`sudo vi install.sh`
To close the file type the esc key then Shift 

`+ :wqa!`

+ Step 5: Change the permissions on the file to make an executable using the command below:

`sudo chmod +× install.sh`

+ Step 6: Run the shell script using the command below. Make sure you read the instructions in the shell script to learn how to use it.

`./install.sh PUBLIC_IP`

## **Deployment of Nginx as a Load Balancer using Shell script**

### _Automate the Deployment of Nginx as a Load Balancer using Shell script_

+ Simplify the process of deploying Nginx as a Load Balancer by leveraging the efficiency of a Shell script. This automation takes you through the seamless deployment and configuration of two webservers, paving the way for a robust load balancing setup.

Here's a brief overview of the process:

1. Prerequisite: Provision an EC2 instance running Ubuntu 22.04
Ensure a smooth start by setting up an EC2 instance with Ubuntu 22.04. This step lays the foundation for the subsequent load balancer configuration.

2. Open Port 80 to Anywhere Using Security Group
Enhance accessibility by configuring the security group to open port 80, allowing seamless communication with the load balancer.

3. Connect to the Load Balancer via Terminal
Once the groundwork is laid, connect to the load balancer effortlessly using the terminal. This step ensures a successful link between your EC2 instance and the load balancer.

## **Effortlessly Implement Nginx Load Balancer: Your Step-by-Step Guide**

+ Unlock the power of load balancing with ease! Our meticulously crafted script encapsulates every detail from the 'Implementing Load Balancer with Nginx' course, providing you a seamless deployment and configuration experience.

+ Explore the script attentively to discover clear instructions on maximizing the potential of your Nginx Load Balancer

### _Steps to Run the Shell Script_

+ Step 1: On your terminal, open a file nginx.sh using the command below:

`sudo vi nginx.sh`

+ Step 2: Copy and Paste the script inside the file

+ Step 3: Close the file using the command below:
type **esc** then shift enter 

`:wga!`
+ Step 4: Change the file permission to make it an executable using the command below:

`sudo chmod +x nginx.sh`

+ Step 5: Run the script with the command below:

`./nginx.sh PUBLIC_IP Webserver-1 Webserver-2`

![Alt text](<Images/Screenshot 2023-12-28 at 9.50.47 AM.png>) ![Alt text](<Images/Screenshot 2023-12-28 at 8.44.46 AM.png>) ![Alt text](<Images/Screenshot 2023-12-28 at 8.44.08 AM.png>) ![Alt text](<Images/Screenshot 2023-12-28 at 8.32.40 AM.png>) ![Alt text](<Images/Screenshot 2023-12-28 at 8.32.34 AM.png>)