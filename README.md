# ![ConVida Project](/images/convida_logo_200x200.png?raw=true)

After COVID-19 crisis, we face a scenario never seen before, all of humanity has been exposed to general confinement and its differences in impact on people will be determined by individual conditions. Everyone will develop an acute stress picture, most without major affectation and with a quick adaptation. The rest of us will have difficulties to overcome the generated stress and this situation will lead to develop a post-traumatic stress disorder (PTSD). Post-traumatic stress disorder is a chronic serious mental illness that needs specialized care in order to overcome it.

## Technical solution

ConVIDA is designed using XX components:
1. Frontend.
2. Doc console.
3. Convida Dialog.
4. Database.

### Convida technical solution

![Convida technical solution](/technical_solution/technical_solution_Diagram.png)

1. The users open Convida web application.
2. In Convida app, Watson assistant is available to do the test.
3. Watson greets the user and invite to do the ASDS test to evalue the level of stress
4. User answer the questions of the form.
5. Functions in Watson evaluates the user's stress level and notify to the user.

## Implemented with:

In this section we have the design of the implemented structure, explaining the various services and the relationship they have with each other.
It can be divided into two blocks:

### mpv 1
We have the list of IBM Cloud resources that we have used to create ConVIDA, of which we have a NGINX server that contains the portal where the chatbot is located.

NGINX is open source web server software.
When someone makes a request to open a web page, the browser communicates with the server of this website. The server then searches for the requested files for the page and sends them to the browser.

Another resource used is the IBM Db2 database to store the results of the tests carried out.

Since the IBM service does not allow the creation of tables but the import, we create the structure of the bd in a virtual machine.
An installation of a docker container was made in said machine in which we installed a DB client to connect to your DB2 instance.
Once the tables are created, we export and import them in IBM db2.

Public services → Cloud Foundry, Apps, Watson Discovery
IBM Watson Discovery is a tool for normalizing, improving, and searching for your unstructured data with speed and precision.
Contains APIs and tools that allow you to easily improve and index large collections of data


### mpv 2

The second block contains the tools to analyze the data obtained from the tests.
We obtain the data from the bd2 and with them we create a dashboard.

A dashboard is a graphic representation of the main metrics or KPIs that are involved in achieving the objectives of a strategy.
KPIs identification: They are indicators that help us measure and quantify work.
These indicators are units of measurement to generate dashboards for the study of health personnel.

1. The dashboard is contained in the administration portal.
2. This portal has an NGINX server to make requests to the browser.
3. The portal is deployed in a delivery pipeline for its development.

Continuous delivery pipeline → It is a development tool that allows to automate the tests so that they can verify the updates of the applications in multiple dimensions before implementing them in the clients.

## How to implement ConVIDA

See [HOWTO.md](howto/howto.md)

## Project roadmap

See [ROADMAP.md](roadmap/roadmap.md)

## ConVIDA Team
* Daniel Franco Puntes 
* Alicia Alvarez García 
* Joan Codina Ortiz
* Adrià Frontana Martínez
* Jesús Pablo Martínez González 

## Acknowledgments

* Kamala Prió
* Carlos Lucas Rodríguez




