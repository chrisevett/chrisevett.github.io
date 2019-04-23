---
layout: page
title: About
permalink: /about/
---

Chris Evett
============

-------------------     ----------------------------
747 Ralph McGill Blvd #1141                                    
Atlanta, GA  
678-551-5568    
chris.evett@gmail.com  
[https://github.com/chrisevett](https://github.com/chrisevett)   
[https://www.linkedin.com/in/chris-evett-22954138/](https://www.linkedin.com/in/chris-evett-22954138/)
-------------------     ----------------------------

Experience
----------

### Senior Manager, Devops ### 
*Steady Platform - March 2018 to present*

**Team leadership and agile coaching**
* As the first engineering hire, worked with developers and product owners to implement agile processes which allowed us to ensure work was flowing through our team. Fostered a culture of continuous improvement and experimentation.   
* Led a team of 3 engineers. Handled product and project management responsibilities for the team. Implemented agile process for project work and internal ticketing for trivial tasks that were not yet automated. Mentored junior engineers and encouraged their professional development.  
* Recruiting and interviewing.  

**Built and operated container orchestration platform**
* Researched and implemented a kubernetes cluster using kops on aws. Built a POC dot net core application to sell the idea of migrating our application to dot net core and kubernetes. 
* Operation of kubernetes cluster. Created manifest templates so that developers could define the environments for their own services so that I wouldn't be a bottleneck for their workflow

**Built and operated CI/CD platform**
* Investigated and implemented a pipeline using drone, helm, and spinnaker allowing applications developers to safely and quickly deliver to production with no downtime. Additionally this allowed us to provide ad hoc environments to developers on demand.  

**AWS management**
* Managed aws account and costs. Saved 3000 USD monthly by migrating staging databases to serverless aurora. Wrote lambdas to schedule backups on ebs volumes and databases based on resource tags. 
* Participated in SOC 2 audit. Ensured that aws resources were compliant using automated systems like aws config. 
* Secured the account using IAM and networking best practices.  

**Observability**
* Built an observability platform using prometheus. Configured alerts and warning to ensure that only true error conditions that required immediate attention were alerted on. Built dashboards to report on non-emergency metrics such as performance, error rates, and throughput.
* Instrumented dot net api to provide application level metrics. Built an integration for a third party analytics platform using golang so we could alert when conditions that would cause customer interaction to descrease occurred.

**etc**
* On call rotation, automation of onboarding tasks, vendor management, organized lunch and learns and events like movie nights and lan parties.



### Cloud Operations Engineer ###
*GE Digital - June 2017 to March 2018*

**Implemented continuous testing tool**
* Wrote a tool in golang that ran inspec tests on the thousands of ec2 instances we were responsible for. Previously we were relying on customer tickets to tell us when our applications were not working as expected.  

**Billing etl application**
* This sounds silly because it is. Using aws lambda, implemented a python application that would consume billing data from azure, and transfer it to s3. Used this as an opportunity to demonstrate python best practices as far as CI/CD and unit testing to the rest of the team.  

**Agile and team development**
* Created kanban process for the team to track project work. Trained team on python and CI/CD best practices. Organized gaming events with the team. Mentored junior developers.  
  
### Site Reliability Engineer ###  
*Cardlytics - April 2015 to June 2017*

**Worked with architecture team to engineer scalable, anti-fragile cloud application**     
* Using terraform, helped to build a scalable and repeatable cloud infrastructure for a pilot application with a high revenue potential.  
* Built a development environment in AWS with a nightly self-destruct in order to minimize the cost of experimentation.  
* Encouraged and helped to implement the '12 factor'-ization of the application and infrastructure to minimize drift and encourage modular work which allowed the team to experiment with and throw away components if needed.  
* Introduced containers into the development workflow which reduced the need for rework after the code was shipped to production due to environmental variation.    
* Led the charge towards 'configuration as code' ideals and helped to enforce it during code reviews.         
* Collaborated with ops team to integrate existing on-prem datacenter resources with cloud resources.  
	   
**Introduced test automation to deployment process**   
* Investigated and implemented a test automation workflow involving test-kitchen, chefspec, and inspec for unit testing and functional testing of chef code.  
* Implemented custom plugins for inspec and test-kitchen to support our specific on-prem datacenter.  
* Integrated TDD workflow into automation provided by our self-service environment portal.  
	
**Automated change control and audit requirements in automated deployments**   
* Integrated jira with octopus deploy in order to facilitate approvals from the business at deploy-time, which enforced rules that were frequently found to be in violation during SOX audits.       

**Provided self-service environments for manual and automated testing**   
* Designed and implemented self-service environment portal using rundeck, ansible, and octopus deploy.   
* Incorporated the portal into the CI process via api calls for use during automated test runs which built quality in to the release process, and eliminated inconsistencies between dev, test, and production environments.
	       
**Implemented chatops health check for common issues in test environments**    
* Using ansible, added monitoring for configuration drift in test environments and made it accessible via a lita.io chat bot so that in many cases app developers and testers no longer had to wait for help when they ran into configuration problems that were blocking their dev/test efforts.
	  
**Training and evangelism**  
* Led efforts to train engineers and business analysts on automation tooling, source control best practices, and test automation for scripting (git/pester/rspec/test kitchen/jenkins).  
* Attended devops conferences and meetups.  
* Lunch and learns and demos of devops tools and principles  
* Organized social activities such as LAN parties and game nights.  

### Software Engineer ###  
*Omnico Group (formerly Matra Systems) - 2012-2015*
* Instrumented POS application with NFC payments capabilities while representing the company as subject-matter expert in communications with clients during the project.
* Streamlined point of sale WCF API, reducing defects in third party client code.
* Provided analysis and detection of defects in device drivers using windows debugging tools, led effort to communicate issues with device vendor to rectify.
* Served as subject matter expert for several products and provided internal training classes for technical teams as well as external demos for customers lacking a technical background.
* Designed and implemented improvements in client code for a coupon management application which eliminated performance issues when consuming a 3rd party API.


### QA Engineer ###  
*Omnico Group (formerly Matra Systems) - 2011-2012*
* Developed a DSL-driven test application for automating functional tests. This turned into a nightly process and a de-facto standard for whether or not a feature was ready to ship.   
* Provided on-site support for testers and product implementation.     
* Designed and executed test plans, documented features.     
* Automated configuration tasks when able. 


Technical skills
----------

#### Programming Languages  
Good at **golang**, **python**, **C#**, **Bash**
Pretty OK at **C**, **C++**, **Python**, **Powershell**, **Ruby**        

#### Tools/ Concepts  
**Configuration Management:** kops, terraform, vagrant, packer, chef, ansible  
**CI/CD:** droneio, spinnaker, travisci, jenkins, appveyor, octopus deploy  
**Etc:** kubernetes, linux, git, prometheus, grafana, vim, regular expressions, docker, nginx, postgresql, mysql, SQL Server, Redgate, IIS, redis, chatops, visual studio, windows server    

### Other accomplishments  

* Speaker at Devops days Atlanta 2017 [Tales of Test-Driven Infrastructure as told by a Windows Toucher](https://www.devopsdays.org/events/2017-atlanta/program/chris-evett/)

* 1st place team 2016 Cardlytics internal hackathon - Attributing spend events to advertisement impressions with mapreduce  

* Finalist TAG 2015 Mobility live [hack-back](http://www.hubga.com/tag-press-release/finalists-revealed-for-mobility-live-hack-back-invitational/) - Dichotomous key for entomology education  

* Various open source contributions. Check out my [github](https://github.com/chrisevett)  

Education
---------

2009
:   **BS Biology**; University of West Georgia
