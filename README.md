# Nessus Installation

# Downloading of Nessus:

- Visit
    
    [Download Nessus](https://www.tenable.com/downloads/nessus?loginAttempted=true)
    
- Download nessus as per your destro
    
    ![Untitled](Nessus_Installation/Untitled.png)
    
    - I am using Kali Linux to demonstrate.

# Installation and Running of Nessus:

- Installation:
    
    ```powershell
    dpkg -i Nessus-10.3.0-ubuntu1404_amd64.deb
    ```
    
    ![Untitled](Nessus_Installation/Untitled%201.png)
    
- Running the Service:
    
    ```powershell
    systemctl start nessusd.service
    ```
    
- Running:
    - Visit:
        
        ```powershell
        https://localhost:8834/#/
        ```
        
        ![Untitled](Nessus_Installation/Untitled%202.png)
        

# Configuring Nessus:

- Choose free version:
    
    ![Untitled](Nessus_Installation/Untitled%203.png)
    
- Enter details:
    
    ![Untitled](Nessus_Installation/Untitled%204.png)
    
    - get temprory mail id from: [https://temp-mail.org/en/](https://temp-mail.org/en/)
- Enter Activation Key:
    
    ![Untitled](Nessus_Installation/Untitled%205.png)
    
- Set Username and Password:
    
    ![Untitled](Nessus_Installation/Untitled%206.png)
    
- It will download all neccessary plugins:
    
    ![Untitled](Nessus_Installation/Untitled%207.png)
    
- Dashboard Access:
    
    ![Untitled](Nessus_Installation/Untitled%208.png)
    

# Running Nessus on Vulnerable Web Application:

- I am Using DVWA as my vulnerable web application
- Using docker image of DVWA: [https://hub.docker.com/r/sagikazarmark/dvwa](https://hub.docker.com/r/sagikazarmark/dvwa)
- My docker image is running on: [http://172.17.0.2](http://172.17.0.2/)

## Setup of Nessus for Scan:

- New scan
    
    ![Untitled](Nessus_Installation/Untitled%209.png)
    
- Web Application tests
    
    ![Untitled](Nessus_Installation/Untitled%2010.png)
    
- Running DVWA docker image:
    
    ![Untitled](Nessus_Installation/Untitled%2011.png)
    
- Set Nessus for the scanning:
    
    ![Untitled](Nessus_Installation/Untitled%2012.png)
    
    ![Untitled](Nessus_Installation/Untitled%2013.png)
    
    ![Untitled](Nessus_Installation/Untitled%2014.png)
    
- Launch the Scan
    
    ![Untitled](Nessus_Installation/Untitled%2015.png)
    
- See in the logs that our scanner in scanning the Application:
    
    ![Untitled](Nessus_Installation/Untitled%2016.png)
    
    ![Untitled](Nessus_Installation/Untitled%2017.png)
    
    ![Untitled](Nessus_Installation/Untitled%2018.png)
    

## SCAN COMPLETED AND FOUND ALL THE BASIC VULNERABILITIES YOU CAN CONFIGURE AS PER YOUR NEEDS

## Contributor:

- [princep4 - Github](https://github.com/princep4)

- [PrincePrafull3 -  Twitter](https://twitter.com/PrincePrafull3)

- [Prince Prafull - Linkedin](https://www.linkedin.com/in/prince-prafull-19a477194/)
