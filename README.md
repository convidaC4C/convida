# ![ConVida Project](/images/convida_logo_200x200.png?raw=true)

## Convid Crisis
After the COVID-19 crisis, we face a scenario never seen before, given that all of humanity has been exposed to general confinement. All will develop an image of acute stress, most without major affectation and with a quick adaptation, but the rest of us will have difficulties to overcome the stress generated and this situation will lead to developing a post-traumatic stress disorder. Post-traumatic stress disorder is a chronic serious mental illness that needs specialized care to overcome it.

We know that confinement causes negative psychological effects, such as stress, confusion, and discomfort. And this thinking of the general population, because there are risk groups, we know that, in healthcare personnel, for all that the Covid-19 entails, they are accumulating a lot of pressure, dedication and fatigue.



## Solution
Our proposal is to minimize people who get sick. For this we present ConVIDA, which is an acronym for (Control variables for the individual diagnosis of Asd (acute stress disorder), ConVIDA is an intelligent chatbot that simulates a real conversation to provide automatic responses to users. Its purpose is to help users people who have generated emotional distress or psychosocial problems triggered by confinement.

ConVIDA will identify the specific problem by using the Acute Stress Disorder Scale (ASDS) test, which is used by psychologists, and provide you with the necessary treatments. ConVIDA will allow us to carry out a screening test to detect people at higher risk of developing post-traumatic stress disorder and to offer them more intensive care.
Wide dissemination through social networks and easy access from any device will ensure that ConVIDA reaches a large number of people.


## Benefit
ConVIDA would improve the mental state of society and we will reduce the most important side effect of Covid-19 which is Health.
COnVIDa will minimize the impact of Covid-19 on the mental health of the general population, while reducing spending on specialized care in national health systems. Furthermore, the team believes that if a functional version comes out in the end and the project is a success, it is easy to create new challenges and continue the project, since it is a problem that covers a lot and new functionalities can be proposed.

I would like to emphasize that, in times of crisis, it is when people need information and answers. It is also when communication with real people is obstructed by causes of the crisis and by a wide need for information, and it is when chatbots are necessary.

People who need professional help will identify in advance and can be helped sooner. COnVIDa, will also help health personnel, friends, colleagues, family members who develop acute stress in their immediate environment, since close people can also develop discomfort from the situation they are experiencing.


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




