---
layout: post
title: "Machine learning model deployment overview"
subtitle: "How to put machine learning models into production
"
date: 2021-09-30 12:00:00 -0400
background: 'img/posts/article1/marta.jpg'
---

You created and validated your machine learning model and now it is ready to create value for your business customers. 

 

The next step now is to integrate your machine learning model into production and make it accessible and available to users and other systems.

In other words **to deploy your machine learning model into the cloud**.

 

Learning how to put your machine learning model into production is an advantage for a data scientist because it requires lots of software engineering and Devops skills. In this article, we are going to overview different ML Model deployment steps and tools.

 

First, we should take into consideration some key questions before we choose our deployment plan as:

How large is your data?

Are you making batch (offline) or real-time predictions?

How do we get feedback from a model in production?

 

These questions are important because they're going to guide you on what Frameworks to adopt for a specific problem.




**1.      create a web application**

 

**API**

 

You just finished your machine learning jupyter notebook, and now you want the user to interact with your code by sending data and receiving predictions. That's why you need **to create an API**.

 

API or application programming interface is a software that allows two programs or applications to communicate with each other to access data Without showing the back end of the software. APIs use specific data formats such as JSON and XML that the two softwares could understand.

In our case here, you want your user to get predictions for your model without showing your code.

 

**Web framework**

 

The problem is that not everyone is familiar with the API structures so we should make it easier for a user to get the predictions from your model without going through the technical side of the APIs. That's why we should build an **end-user framework** too.

 

Examples of tools you can use to build a ML application with both an API and an end-user framework are **Flask, streamlit and Django**.

 

**Flask** is a web framework Written in Python that provides you with tools, libraries, and Technologies to build a web application.

It needs some knowledge on HTML and JavaScript to create the front end for your application with Flask.

Flask is a lightweight web framework, so it has a limited capacity to handle complex applications which make it more suitable for only single page applications, 

 

**Streamlit** is an open-source Python library that makes it easy to create and share beautiful, custom web apps for machine learning and data science. In just a few minutes you can build and deploy powerful data apps.

 

**Django** is a high-level python web framework that enables rapid developments of secure and maintainable websites. Django was designed for fast development of complex web apps, so it has more additional features than Flask.




 

**2.      Containerize your model**

 

Now the web application is running perfectly on your local machines but when you share it with someone else, it doesn't work maybe because of missing dependencies in his Jupiter environment, or he is using a different OS. The solution here is **to Containerize your application.**

 

“What Does Containerization Mean? 

Containerization entails placing a software component and its environment, dependencies, and configuration, into an isolated unit called a container. This makes it possible to deploy an application consistently on any computing environment, whether on-premises or cloud-based.” [aquasec.com](https://www.aquasec.com/cloud-native-academy/docker-container/container-devops/)


 

Platforms that offer this service are **Docker** and **Kubernetes**.

 

**Docker**

Docker is an open platform for developing shipping and running applications. It enables you to separate your application from your infrastructure and be able to run your application in any other environment.

If we are able to run our code without any problems in our docker container, we can run it anywhere and prevent the problem of “it worked on my machine!” 

 

**Kubernetes**

Kubernetes is an open-source container orchestration platform for scheduling and automating the deployment management and scaling of containerized applications.

 

Kubernetes include a masternode that schedules the workloads for the rest of the containers in the cluster, so it enables the management of high volumes of containers through their life cycles.

 

One example of Kubernetes' advantages is its load balancing and autoscaling, which means that Kubernetes automatically starts up new containers to handle heavy loads from users.

 

You can choose one of those options or you can combine both and choose Docker as a container in the Kubernetes platform.




**3.      Deploy your model into the cloud**

 

It's time to deploy your machine learning model into the web and make it accessible to other users using an URL.

We can use one of the following platforms to deploy our models in the clouds:

 

**Heroku** is a cloud platform as a service ‘PAAS’ that helps you deploy, manage and scale your applications without complex infrastructure.

You can easily upload your trained machine learning model into Heroku by linking your GitHub repository to your Heroku account.

 

**Google app engine** is a cloud computing platform as a service for developing and hosting web applications in Google managed data centers.

 

**AWS Elastic Beanstalk** is a platform as a service provided by AWS, used for deploying and scaling web applications.

 

**Azure Web Apps** a fully Managed web hosting service for building Web, mobile and API applications.

 

Once you follow these 3 steps, you have a public URL where you can share your ML app with your users.

 

**Conclusion**

 

Creating a good machine learning model is great but not enough to create value, we should also make it into production for a real Business use case.

I hope this article gave you a clear idea on some ways to deploy your model into the cloud.

 