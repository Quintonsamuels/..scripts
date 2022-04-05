# ELK STACK PROJECT 
This Repository consist of lynix script soultions that Ive covered in this course and also solutions to creatiing a CLOUD NETWORK that is presented in the link below.. 
(https://user-images.githubusercontent.com/94322084/161686299-1724d2db-74b2-432d-8c0d-e39932900499.png)         

the files have been tested and used to generate a live ELK deployment on Azure, and can be use to create another deployment of the image above.
in order to install portions of the ansible file (click the links below).

### Enter Ansible File

-https://github.com/Quintonsamuels/..scripts/tree/main/ansible

The following details are located in this file:
- HOW TO ANSIBLE THE BUILD 
- POLICIES ACCESS
- Description of the Topology

### ELK Configuration 

Using Ansible to automate configuration of the ELK machine. There is an advantage becuase nothing was carried out manually, So the system updates can be used 
expertly 

the following 5 steps are used to Install ELK, Install Docker & etc. :
- - name: set maximum map count in sysctl/systemd
- - name: docker.io
- - name: instal pip3
- - name: Install Docker module
- - name: download and launch elk

The scripts above list the solutions  of running "docker.io" after configuring the ELk instance successfully.

### Access Polcies 

Do to the internal Network the machines are not exposed to the public internet.
only the jumpbox machine is capable to connect to the internet, But to access the machine you must be allowed through the IP addresses.

- The Jump-Box-provitioner is able to connect via SSH to the Elk-Stack machine through port 22. In addition the Personal Host IP address is also able to access the Elk-Stack    machine through port 5601


A summary of the access policies in place can be found in the table below.

| Name     | Publicly Accessible | Allowed IP Addresses  |
|----------|---------------------|-----------------------|
| Jump Box | Yes                 | Public IP, 10.0.0.4   |
| Web-1    | No                  | 10.0.0.5              |
| Web-2    | No                  | 10.0.0.6              |
| ELK-Stack| yes/No              | Public IP, 10.1.0.4   |
| Load-bal | Yes                 | 20.124.200.176        |

### Description of the Topology

The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.

Load balancing ensures that the application will be highly available , in addition to restricting access to the network.

The load balancer protects against DDoS (Denial of service) attacks, SSL offload, authenticate user ID, protects applications from threats, traffic compression, and traffic cashing.
  
 Acts as an audit for traffic and a single point where we can manage user accounts.

Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the data and system logs.

 The configuration details of each machine may be found below.


| Name     | Function         | IP Address | Operating System |
|----------|----------------- |------------|------------------|
| Jump Box | Gateway          | 10.0.0.4   | Linux            |
| Web-1    | Server           | 10.0.0.5   | Linux            |
| Web-2    | Server           | 10.0.0.6   | Linux            |
| ELK-Stack| monitoring Server| 10.1.0.4   | Linux            |





