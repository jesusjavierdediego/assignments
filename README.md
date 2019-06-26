![Assignments](assigments.jpg)

# Introduction
Congratulations! You have been selected for the next phase of the selection process: The assignment.

This phase consists of the making of a small software project. The true objective of this task is to have an opportunity for a discussion about your technical skills as well as your approach to the solution of software engineering problems.

There are three options. You should pick up one only. Regardless what is your assignment you should follow always the same criteria:

## 1-Write the Requirements
You are in charge and you formulate the specific requirements. Use Functional (FR) and Not Functional Requirements (NFRs) in your wish list. For instance performance, responsiveness, concurrency, etc although some times you'll see some NFRs in the description of the assignment.
We strongly recommend you using the Gherkin syntax to write the requirements (FRs and NFRs). Never forget to attach your Gherkin test scenarios to real working testing code in your assignment.

## 2-Follow a Quality Driven Methodology
Write the code following the procedure, methodology and quality approach you consider is the best one for your project. Please include comments to illustrate decisions, solutions and approaches. 
We recommend you to pay special attention to the structure of the project, segregation of tasks and clarity of the code.

## 3-Be explicit
Please illustrate your assignment with additional information. We're interested on your approach to solve problems.

## 4-Technological Landscape
Please have a look on our ![flyer](https://devportal.fexcofts.com/pdf/FTS-advert-office.pdf). You can find in there the set of tools and technologies we are interested on. This is important as we are already working with this stack.

## 5-Common Rules
Some essential things are expected by default. Git, Git workflows, quality, automated testing (TDD and BDD), knowledge about networks, infrastructure, computing, network protocols, SDLC, ALM, etc are common terms in the software engineering world. Please review your assignments accordingly to this common language by considering these aspects in your introduction.

## 5-The Assignment Session. You're the star!
We'll meet and you'll start with a short presentation (around 15 minutes) explaining the requirements your wrote, your plan for the project, your approach to the problem, your quality criteria and tools and so on. It would be ideal if you show how your project actually works. Be brief and prepare the introduction to your assignment previously. You can expect some questions about specific details in code, organization, technical decisions, architecture or the followed approach.

After your presentation we'll have a brief discussion about your work and we'll ask some questions from your code. It's simple!



Let us remind you some key concepts about how to take the assignment phase:

**Honesty**

Remember the goal is to give us an idea of your personal and special way of understanding software development. Please be honest and write your own code. Follow an original approach as well. What we want is to read YOUR code even with possible errors or mistakes and errors rather than reading copied/pasted code from someone else. Besides, if we detect any copied snippet it will be really embarrassing.


**You're special**

We do not expect here another Spring-based project (no, not again!). Be original, follow your instinct and plan something new. It is not perfect, it is clearly improvable. Well, it is not a problem to us. The case here is to show us your skills to solve probelms and the ability to carry out a software project based on high quality standards while providing agility, performance and efficiency.


**Think of the whole process**

Try not thinking as a pure developer whose concern is only to write functional code and nothing else. We prefer the term **Development Engineer**. The Engineer is aware of the whole **Software Development & Delivery Life Cycle** to provide the maximum quality of the software as well as the integration of the tools to bring the component to Live considering all the circumstances in a regular delivery pipeline as well as having in mind the underlying infrastructure that will support your software.


**Read everything!**

Have a look below on the different options for assignments and choose your favourite one. Please read carefully all the sections in the chosen assignment option to avoid confusions. 


**Any doubt?**

Do not hesitate to send us your questions to clarify any aspect of the assignment or the methodology.

For any question send an email to jdediego@fexco.com, fmuno@fexco.com or tmacsweeney@fexco.com

Besides, you can read our [FTS Techblog](https://techblog.fexcofts.com/) to be more familiar with our points of view. 




# Assignments

## Option 1: The API and the Front-End Consumer

### Description
In this assignment our mission is to produce an API server that will expose 2 or more endpoints or services. These endpoints will implement some regular CRUD functions with data to be consumed by a public API consumer (e. g. a public web site).



### Special Rules
- Well, usually API endpoints are based exclusively on a single protocol, HTTP1. However, our API is intended to support at least two protocols. We suggest to publish a subscription to a topic for notifications or creating some streaming channel based on HTTP2. 
- Regarding multi-protocol APIs you can have a look on [this post](FTS-advert-office.pdf).
- Some examples of protocols for an API are: HTTP1, HTTP2, AMQP, MQTT, etc.
- In any case the client (we prefer the term *API Consumer* ) should consume somehow all the endpoints available in the API regardless the implemented protocol.
- It is not needed that every endpoint in the API server implement several protocols. 1 protocol per each endpoint is OK. For instance, your service has three HTTP endpoints for CRUD and 2 AMQP endpoints for notifications and alerts. That would be OK to us.
- Remember: DONE MEANS RELEASED! The assignment target is to provide a released component or component to Live.This rule has to be a constant in your assignment. 


### Requirements
- We expect a concurrency of 50 users (24/7) with an average user operation duration of 10 minutes.


### Expected Deliverables
We'd like to see:

1-The API server implementing the multi-protocol endpoints. Solutions, approaches, usages.

2-An API consumer that actually does something with the API endpoints, composing and showing information retrieved from the API, asynchronously receiving real-time information, etc.

3-Any IaC needed to see everything working (optional, it's an extra). However, for demo purposes it can run on your machine as the default option.



## Option 2: Multi-Distribution Front End Application

### Description
This case is peculiar as it is focused on the Front End side of things. However, this is not about a common regular JS webapp or something like that. We're talking here about a complete killer app that will be distributed in different flavours: web, desktop and mobile.

### Special Rules
We're interested about how you consume an API (of course) but the target here is your ability to design and develop the whole distribution set of an app. Please read carefully the requirements below.
E2E, and all types of functional and not functional tests are dramatically important. Do not forget to include them into the assignment.
The number of features can small but all of them have to be completely covered by quality rules and tests. The 


### Requirements
1-Web version. The app can be accessed via most used web browsers with no loss of features: Firefox, Chrome, Safari, Edge.

2-Desktop version. The app is distributed with a desktop version. That means it has to be able to be downloaded and installed to desktop main OSs (Windows and Linux). 

3-The app has to be able to remain functional even when there is not connection to Internet. Yes, we mean offline features. Besides, the app has to be able to detect the cnnection is available again and synchronize data with the Back End.

4-Usability and User Experience are key aspects. The app has to be easy and intuitive for not-trained users.

5-How to display large amounts of data. The app will show somewhere a long list of records. The list has to be responsive, low-latency and really easy to use.

6-Mobile app. The app should be ready to be published to main mobile app stores (Google Play and Apple Store). The model can ca hybrid or native.

7-SDLC for a multi-target distribution can be complex. Please include in your assignment your preferred approach for this area as well as a basic implementation at least.


### Expected Deliverables

1-Web applictaion

2-Desktop appliation

3-Mobile application 

4-SDLC proposal and basic implementation (minimum)



## Option 3: Extract, Transform, Load large amounts of data

### Description
Probably you've guessed the main topic of this assignment from the header. Yes, it's about the infamous ETL processes world. The assignment consists of the making of an ETL applications that esentally:

1. It gets the data from a source data storage.
2. It applies one or several transformations of the content or the formats in a meaningful way that cost some processing time.
3. Finally, it loads the result of the transformation to a one or several destination data storages.


### Special Rules
- The application will run in a nightly basis with a limit of 15 minutes of running time (this is the time window provided by the evil people in charge of the infrastructure).
- The maximum amount of memory to be consumed by the application is 2.5 GB (again, that evil people).
- Our system is 24/7. So, the source data storage can not suffer any latency or issue derived of the query related to the Extraction phase.


### Requirements
- The ETL process must be able to handle at least `2 million of records` for all involved phases.
- We expect notifications from any unexpected error.
- The ETL process should log all actions at different levels of importance and priority.
- Administrators should be able to compose graphical dashboards from the operation logs of the ETL process in time. 


### Expected Deliverables
We'd like to see:

1. The ETL application including the mentioned phases as well as mock data storages to test the component. You can use publicly available sources of data, public files with data, etc.
2. Any related component handling the traces and logs from executions
3. Any IaC needed to see everything working (optional). It can run on your machine as the default option.




## Option 4: A Microservice in Kubernetes

### Description
The goal of this assigment gathers a software component with IaC. Our mission is to develop an application as a microservice, following the main guidelines of the Micro Services Architecture (MSA). There is not any requirement about the implemented protocols but we'd like to see here is a good, solid, robust and efficient microservice, completely autonomous and containing all the features we could find in the best examples of microservices around the world.

Besides, we should release our microservice in a Kubernetes cluster and find out what is its behavior in a Kubernetes pod with several containers containing the app.
Kubernetes deployment should adapt to the load by creating / destroying containers when the load grows.

The load to test the system should apply a load ramp as in the picture:

![LOAD RAMP](load.png)


### Special Rules
- You can choose your favourite protocol or protocols for the microservice but you always should follow an architectural pattern (for instance, REST architecture for HTTP1). 


### Requirements
- High Availability, responsiveness and robustness are the core terms in this assignment. It is expected a really high concurrency (+500 users) and workload (heavy payloads with hundreds of KBs in some occasions). 
- You should implement some kind of heavy payload in the usage of the microservice to emulate this workload.
- We expect to see the number of microservice instances to grow from 2 (initial configuration) to N where N is what you need to cope with the maximum load. After 10 minutes of stress test (as described in the diagram) the system should return back to normal. If your microservice handles perfectly the load just with 2 instaces, please include a configuration option that degrades the preformance of the microservice so that we can see this growth.


### Expected Deliverables
1. The microservice application applying all the special rules and standard quality features that are expected in Enterprise MSA.
2. This time is not optional: `You have to provide the IaC needed to stand up a Kubernetes cluster` with a pod of several instances of the microservice. The target of the IaC can be a Cloud Provider or anything you consider. Factors as exchangeability, agnosticism and versatility of the IaC code will be really appreciated.
3. A stress tool log report showing the performance evolution of the global system (Jmeter, Soap UI or any other you like)
 

**Good Luck!**

Well, that's all. Again, if you have any question send an email to jdediego@fexco.com, fmuno@fexco.com or tmacsweeney@fexco.com

