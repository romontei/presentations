# Deploy application hosted in the cloud using lambda functions

# [See this post](https://medium.com/swlh/serverless-architecture-complete-reference-guide-2019-55363c08d1be)

## Serverless 

Serverless computing is a cloud-computing execution model in which the cloud provider runs the server, and dynamically manages the allocation of machine resources. Pricing is based on the actual amount of resources consumed by an application, rather than on pre-purchased units of capacity. 

Most but not all serverless vendors offer compute runtimes, also known as function as a service (FaaS) platforms, which execute application logic but do not store data. The first "pay as you go" code execution platform was Zimki, released in 2006, but it was not commercially successful.
In 2008, Google released Google App Engine, which featured metered billing for applications that used a custom Python framework, but could not execute arbitrary code.
PiCloud, released in 2010, offered FaaS support for Python.

AWS Lambda, introduced by Amazon in 2014, was the first public cloud infrastructure vendor with an abstract serverless computing offering. It is supported by a number of additional AWS serverless tools such as AWS Serverless Application Model (AWS SAM) Amazon CloudWatch, and others.

Google Cloud Platform offers Google Cloud Functions since 2016.

IBM offers IBM Cloud Functions in the public IBM Cloud since 2016.

Microsoft Azure offers Azure Functions, offered both in the Azure public cloud or on-premises via Azure Stack.

Oracle introduced Fn Project, an open source serverless computing framework offered on Oracle Cloud Platform and available on GitHub for deployment on other platforms.

In addition, there are a number of open source serverless projects with various levels of popularity and usage:

OpenWhisk was initially developed by IBM with contributions from RedHat, Adobe, and others.
OpenWhisk is the core technology in IBM Cloud Functions.

Project Riff is an open source serverless platform implementation built on Kubernetes by Pivotal Software. Project Riff is the foundation of Pivotal Function Service.

## Lambda functions

Lambda functions are executable functions that are hosted on AWS that only run whenever you invoke or call the Lambda. They can be written in a range of languages including C#, JavaScipt (through Node.js), Python 2 and 3, Go and Java. This means you can do really cool things like having a JavaScript stack but with a Python Lambda for machine learning or Go for running compute expensive tasks.

One of the major advantages of Lambdas is that you are only charged for the time it takes for the function to run. This means that functions that are called once every 10 minutes and take 2 seconds to run are charged for just 288 seconds per day (144 times a day x 2 seconds). That equates to 0.17 cents a month or $0.02 a year!

Another advantage of working with Lambdas is that they automatically scale at no extra cost. This could be scaling over time as your product grows as well as scaling up and down with the usage cycles throughout the day. If you have a Lambda that gets hit a lot throughout the day but less overnight then the Lambda will automatically provision the resources you need. This means that you aren’t wasting money on resources that are just sitting idle overnight, but won’t get server crashes if there is a user spike.

<img src="https://miro.medium.com/max/2556/1*6rMn8P7AxpjOpHg_7vTUAQ.png"></img>

# Avantages

- Aucune gestion de l’infrastructureAucune gestion de l’infrastructure
- Scalabilité dynamique
- Time-to-Market plus rapide
- Utilisation plus efficace des ressources
- Cost

# Inconvenient

- Testing and debugging become more challenging
- Serverless architectures are not built for long-running processes
- Vendor lock-in is a risk



