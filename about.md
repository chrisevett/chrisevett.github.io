---
layout: page
title: About
permalink: /about/
---

Chris Evett - automation, devops, kaizen, and continuous everything
============

------------  
Atlanta, Georgia  
Email:chris.evett@gmail.com  
Github:[chrisevett](https://github.com/chrisevett)  
Twitter:@chris_evett
 
-------------

Experience
------------


# Site Reliability Engineer - Cardlytics 
*April 2015-present*      
  
**Worked with architecture team to engineer scalable, anti-fragile cloud application**     
  - Using terraform, helped to build a scalable and repeatable cloud infrastructure for a pilot application with a high revenue potential.  
  - Built a development environment in AWS with a nightly self-destruct in order to minimize the cost of experimentation.  
  - Encouraged and helped to implement the '12 factor'-ization of the application and infrastructure to minimize drift and encourage modular work which allowed the team to experiment with and throw away components if needed.  
  - Introduced containers into the development workflow which reduced the need for rework after the code was shipped to production due to environmental variation.    
  - Infrastructure was built immutably which removed the need for traditional handoffs between dev, test, and ops in order to ship code.
  - Led the charge towards 'configuration as code' ideals and helped to enforce it during code reviews.         
  - Implemented blue-green deployments into the application using elastic beanstalk and elastic container service so that changes could be made to production with zero down time.  
  - Collaborated with ops team to integrate existing on-prem datacenter resources with cloud resources.  

**Led kanban and devops transformation of a legacy-app development team**   
	- Introduced a structured kanban process to a previously interrupt-driven team.    
	- Worked with developers and tech director to focus on delivering value to the business instead of fighting fires.  
	- Implemented a proactive weekly iteration of work that was planned instead of solely responding to bugs and outages. Introduced retrospectives and blameless post-mortems into the team workflow in order to increase feedback on how the team was working.
	   
**Introduced test automation to deployment process**   
	- Investigated and implemented a test automation workflow involving test-kitchen, chefspec, and inspec for unit testing and functional testing of chef code.  
	- Contributed to and created OSS projects to support automation pipeline **See my github at the top**  
	- Implemented custom plugins for inspec and test-kitchen to support our specific on-prem datacenter.  
	- Greatly increased speed of deployment code implementation by introducting TDD-style workflow to the team.  
	- Integrated TDD workflow into automation provided by our self-service environment portal.  
	
**Automated change control and audit requirements in automated deployments**   
	- Integrated jira with octopus deploy in order to facilitate approvals from the business at deploy-time, which enforced rules that were frequently found to be in violation during SOX audits.       
	    
**Source controlled and containerized CI server configuration**  
	- Migrated on prem CI server off of manually configured 'snowflakes' that had to be restored from backups in the event of catastrophe, to containerized applications where 100% of configuration was source controlled. This allowed us to quickly experiment with different configurations without worrying about affecting 'production' build activity.  
	    
**Provided self-service environments for manual and automated testing**   
	- Designed and implemented self-service environment portal using rundeck, ansible, and octopus deploy.   
	- Incorporated the portal into the CI process via api calls for use during automated test runs which built  quality in to the release process, and eliminated inconsistencies between dev, test, and production environments.
	       
**Implemented chatops health check for common issues in test environments**    
	- Using ansible, added monitoring for configuration drift in test environments and made it accessible via a lita.io chat bot so that in many cases app developers and testers no longer had to wait for help when they ran into configuration problems that were blocking their dev/test efforts.
	     
**Built custom inventory plugin for legacy monitoring application**  
	- Integrated solarwinds with a custom dot net plugin in order to identify servers and the applications that ran on them on a centralized system . 
	  
**Training and evangelism**  
	- Led efforts to train engineers and business analysts on automation tooling, source control best practices, and test automation for scripting (git/pester/rspec/test kitchen/jenkins).  
	- Attended devops conferences and meetups.  
	- Lunch and learns and demos of devops tools and principles  
	- Organized social activities such as LAN parties and game nights.  
  
# Software Engineer - Omnico Group (formerly Matra Systems) 
*2012-2015*  
	- Overhauled windows installers (batch/VBS/Jscript and WiX/msi).  
	- Maintained legacy point of sale application  
	- Lots of boring projects that taught me how not to develop software and made me realize the importance of automation, quality, and communication. 
  

# QA Engineer - Clarity Commerce (formerly Matra Systems) 
*2011-2012*  
	- Developed a DSL-driven test application for automating functional tests. This turned into a nightly process and a de-facto standard for whether or not a feature was ready to ship.   
	- Provided on-site support for testers and product implementation.     
	- Designed and executed test plans, documented features.     
	- Automated configuration tasks when able.  


Technical skills
--------------------

#### Programming Languages  
Good at **C#**, **Powershell**, **Ruby**, **T-SQL**  
Pretty OK at **Bash**, **C**, **C++**, **Python**, **VBScript**    


#### Tools/ Concepts  
**Configuration Management:** chef, ansible, powershell DSC  
**Environment automation:** rundeck, terraform, vagrant, packer  
**CI/CD:** jenkins, teamcity, bamboo, travis ci, appveyor, octopus deploy  
**Test Automation:** test kitchen, rspec, inspec, chefspec, nunit, selenium, pester    
**OS:** Centos, Ubuntu, and Windows server.  
**Etc:** git, bitbucket server, github, vim, artifactory, regular expressions, docker (windows and linux), nginx, SQL Server, Redgate, wix, IIS, redis, azure service fabric, chatops, visual studio    

### Other accomplishments  

* Speaker at Devops days Atlanta 2017 [Tales of Test-Driven Infrastructure as told by a Windows Toucher](https://www.devopsdays.org/events/2017-atlanta/program/chris-evett/)

* 1st place team 2016 Cardlytics internal hackathon - Attributing spend events to advertisement impressions with mapreduce  

* Finalist TAG 2015 Mobility live [hack-back](http://www.hubga.com/tag-press-release/finalists-revealed-for-mobility-live-hack-back-invitational/) - Dichotomous key for entomology education  

* Various open source contributions. Check out my [github](https://github.com/chrisevett)  


### Education  
BS Biology major Math minor, University of West Georgia 2009  
Graduate coursework in Biology, Georgia Southern University 2009-2011  
Coursework in Computer Science, Oregon State University 2015  
