---
layout: post
title: "Notes from velocity 2016 new york"
comments: true
description: "Brief summary of some of the takeaways forom 2016 velocity"
keywords: "velocity, new york, 2016, continuous delivery, devops"
---


### process changes   
nonfunctional requirements such as automation ,security, quality/tests should be in the definition of done  
try and get some of this into our dev workflow [https://alexgaynor.net/2015/may/27/tips-for-scaling-web-apps/]()


### tools to investigate 
Linkerd [https://linkerd.io/](Linkerd.io)  
Namerd  
HAProxy  
Sql server HA/ dark deployments  
Dev strategy for dark sql deployments (turn it on in the DB, then turn it on in the app)  
See if these are open source, dropbox tools Dbmanager, wheelhouse, naoru  
dh2i sql containers  
DOCKER DOCKER DOCKER DOCKER DOCKER    
docker jenkins pipeline.   

### things to read/ watch 
kmod on scale dropbox youtube video  
stackoverflow tech blog  
netflix tech blog  

### things to build
cli tool to set up build/deploy and also local dependencies for .net apps like netflix newt

### other todos
Come up with a study syllabus for gaps in code (go and ruby) , linux (admin tasks, security) , tools (docker, mesos, vim, hashicorp, dc/os, etc) , networking(maybe ccna stuff?) in that order. Forget about databases Check everything in as code.  
Come up with a plan to execute it. Remember small batches, small goals, MVP of learning. First milestone is the syllabus, second is starting the process. Find a study buddy.  



### takeaways from talks 

#### Limoncelli from stackoverflow  

Apply devops principles to things that aren't SDLC
Principles:    


- The three ways  
- Systems thinking  
- Rapid Feedback loops  
- Kaizen culture/ encouragement of continuous improvment  
- Minimum viable product delivered as soon as possible (definition of product is loose)  
- Small batches  

An example of a devops principle (small batch in this case) applied to something is the decision to give constructive feedback early in a relationship instead of letting frustrations and differences accumulate.  
Also he used weightloss as an example. He set the goal to lose one pound per week instead of 100 lbs in a year.  Whenever there were failures he would analyze the situation and make corrections and the weightloss stuck.  

System integrity is more important than the actual system. If you don't **know** that it's working then the business isn't getting value from it.   

Automate acceptance tests and testing of nonfunctional requirements (eg infra testing. The infrastructure as code guy said the same thing). Does this apply to monitoring and test automation?  

#### Soundcloud load balancing talk 

Soundcloud load balances their internal apps. Their load balancer of choice is HAproxy.  
HAProxy is an excellent source of metrics. nginx is not  
The ended up using dns service discovery for their microservices. It was the most scalable solution because they couldn't handle all of the configs iirc. It removed the IP layer of balancing.    

#### The ex twitter guy talking about the layer 5 routing   
The problem this guy was solving was that everyone had to configure timeouts/ retries/ etc for their web/db connections. The solution was to build a library that handled all layer 5/ session level config so the code could just worry about level 7 / app layer  
Twitter library is finagle    
Linkerd is an open source version of this that might be useful, does service discovery and service management  
Namerd is a routing service, does the balancing that sat on top of the haproxy balancers in the soundcloud talk (in general)  

#### Dropbox databases
All database changes are done in code (something like entity framework) so nobody writes sql.  
They roll alot of their own tools in go   
MySql everything. They recently rolled out a MySql wrapper that abstracts the database details.  
Sharding and splitting of databases when complexity becomes unwieldly  
Tools for managing deployments: Dbmanager, wheelhouse, naoru, see if these are internal or open source  
Sqlproxy, proxysql, whatever its called. Investigate and see if we can find something similar for mssql  
There is some sort of container wizardry they do. Reconsider dh2i or whatever the microsoft sql analogue is  

#### netflix containers 
Netflix originally baked their apps into vm's using spinnaker  
The use case for containers was long running batch jobs. Just run til done we dont gaf about it  
Ad hoc reports done in containers.  
Benefit of containers is that we can run it on spare infra  

Use a container service on each AMI/vm that tells each container what to be.  They had to do some faking  

New tool is a cli tool that sets up vagrant virtual box and dev dependencies. Remotely it set up jenkins job, spinnaker project, artifactory repo, etc  

They test their libraries the way i should test infrastructure. 

#### Infrastructure as code guy 
Nothing really new here. Seems like I have all the right ideas except for databases which he didnt cover .

JFDI Cowboy vs beaurocrat ideology is toxic. Change should be encouraged but quality should be enforced.  

Goal is the ability to make quick change with confidence.

Quality and compliance can be validated on every change. Good use case for inspec for compliance. 

Set up chef agents to apply config changes continuously (in prod? maybe when we're mature)

Immutable infrastructure. All changes are a new server. A sane alternative is using containers and replacing them .  


### ideas from last time, things i recapped on, ideas for current projects 
20% of dev time should be committed to nonfunctional features eg infra, tests, monitoring  
Load balance and cluster internal apps   
security: whenever someone has to log in to something make an effort to deprecate that need (use automation/self service to solve their problem)  

#### Things I can try
Dark deploy features  
Load balanced HA setup  
HA database setup so we can do automated deployments and dark releases  
Use replication  
In the publishing queue the redis cluster is only utilizing one node    
Sharing/splitting databases that are tarded  
dh2i   
jenkins chef and docker it   
practice failing over monthly   
goal should be 0 downtime    
blue green turquoise for databases  

