# How to implement ConVida:

## Set up Nginx Web Server with Cloudfoundry

Based on [https://developer.ibm.com/tutorials/cl-deploy-a-hello-world-webpage-to-bluemix-app/](https://developer.ibm.com/tutorials/cl-deploy-a-hello-world-webpage-to-bluemix-app/)

The manifest of the Webserver can be viewed [here](https://github.com/convidaC4C/convidaC4C_frontend/blob/master/manifest.yml) and the code of the web page is the repository [convidaC4C_frontend](https://github.com/convidaC4C/convidaC4C_frontend).



## Set up Watson Assistant

Follow the instructions of [this manual](https://github.com/Call-for-Code/Solution-Starter-Kit-Communication-2020/blob/master/README.md#set-up-an-instance-of-watson-assistant) until step 5.

Then we have created a new skill to do a form based on the ASDS test, the json associated is this [skill-COnVIDa-MVP](skill-COnVIDa-MVP-copy.json).


## Set up DB2 Database

### Local db2 docker creation
__Step 1:__ Linux installation
We have used an LTS version as it is a stable version of the Linux based Ubuntu operating system which is mainly aimed at enterprise level server environments.

As well as having a lot of documentation and compatibility.
Follow the instructions of [this manual](https://releases.ubuntu.com/18.04.4/)


__Step 2:__ Install Docker Engine on Ubuntu
Follow the instructions of [this manual](https://docs.docker.com/engine/install/ubuntu/)

In Installation methods we have performed the installation using a repository.


__Step 3:__ Download the DB2 DB image
Follow the instructions of [this manual](https://hub.docker.com/_/db2-developer-c-edition)

In section "Getting Db2 Developer-C image" we have used the image db2_developer_c:11.1.4.4-x86_64



__Step 4:__ Install a DB client to connect to your DB2 instance
We downloaded a java engine to make dbeaver work.
We use the java jdk openjdk-11-jre-headless.

Once the DB2 server is installed, we need a client with which to design the databases.
We use dbeaver which we download [here](https://dbeaver.io/download/), download the debian image(Linux Debian package 64 bit (installer))
 
 
### Use of dbeaver to design data ta

### How to exporting table data to CSV format
__Step 1:__ Select a table you want to export. In the context menu choose "Export Data".

__Step 2:__ Choose export format. DBeaver support many different output formats including CSV, HTML, XLSX, etc

__Step 3:__ Set data extraction options. This may affect extraction performance

__Step 4:__ Set export format option. They are specific to the data format you choose on Step 2

__Step 5:__ Set options for output files or clipboard

__Step 6:__ Review what and to what format you will export

__Step 7:__ Press finish. See extraction progress. 


### DB2 instance creation in ibm cloud.

### Importing tables to the DB2 instance in ibm cloud.
