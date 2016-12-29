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
----------

**Devops/Automation Engineer - Cardlytics** April 2015-present    

**Transformed a business-critical legacy app from a manual deployment requiring downtime to a continuous deployment with 0 downtime**   
  - Replaced former application set up for which deployments were high risk and required hours of downtime and revenue impact for a single deployment with a highly available web server architecture  
  - Collaborated with development team to change database development practices to enable a "blue-green-turquoise" deployment strategy which completely eliminated downtime during deployments  
  - Moved from using 0 source control for configuration to source controlling all of the configuration for that application  
  - Moved from 0 deployment automation for this app to using chef for config management and deployment and test-kitchen for test automation of chef code.     
**Introduced test automation to deployment process**   
	- Investigated and implemented a test automation workflow involving test-kitchen, chefspec, and inspec for unit testing and functional testing of chef code.  
	- Contributed to and created OSS projects to support automation pipeline **See my github at the top :)**  
	- Implemented custom plugins for inspec and test-kitchen to support our specific infrastructure.  
	- Greatly increased speed of deployment code implementation by introducting TDD-style workflow to the team.    
**Source controlled and containerized CI server**  
	- Migrated on prem CI server off of manually configured 'snowflakes' that had to be restored from backups in the event of catastrophe, to containerized applications where 100% of configuration was source controlled.    
**Provided self-service environments for manual and automated testing**   
	- Designed and implemented self-service environment portal using rundeck, ansible, and octopus deploy.   
	- Incorporated the portal into the CI process via api calls for use during automated test runs which built  quality in to the release process, and eliminated inconsistencies between dev,test,and production environments.       
**Built health check for test environments for common issues**    
	- Using ansible, added monitoring for configuration drift in test environments and made it accessible via a lita.io chat bot so that in many cases app developers and testers no longer had to wait for help when they ran into configuration problems that were blocking their dev/test efforts.     
**Shored up ipaddress management practices**  
	- Migrated ip address management for on prem vsphere host from a spreadsheet with tabs for each subnet to an open source tool with an API. This tool was later utilized for dynamic assignment/release of static IP addresses during environment automation.  
**Training and evangelism**  
	- Led efforts to train engineers and business analysts on automation tooling, source control best practices, and test automation for scripting (pester/rspec/test kitchen).  
	- Attended devops conferences and meetups.  
	- Lunch and learns and demos of devops tools and principles  
	- Organized social activities such as LAN parties and game nights.  
     
  
  
**Software Engineer - Omnico Group (formerly Matra Systems) 2012-2015**

- Overhauled windows installers (batch/VBS/Jscript and WiX/msi).  
- Maintained legacy point of sale application
- Lots of boring projects that taught me how not to develop software and made me realize the importance of automation, quality, and communication. 
  

**QA Engineer - Clarity Commerce (formerly Matra Systems) 2011-2012**

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
**Environment automation:** rundeck, vagrant, terraform, packer  
**CI/CD:** jenkins, teamcity, bamboo, travis ci, appveyor, octopus deploy  
**Test Automation:** test kitchen, rspec, inspec, chefspec, nunit, selenium    
**OS:** Linux (RHEL/Debian) and windows (2003+).
**Etc:** git, bitbucket server, github, vim, artifactory, docker, nginx, SQL Server, Redgate, wix, IIS, redis, azure service fabric, chatops

### Other accomplishments  

* 1st place team 2016 Cardlytics internal hackathon - Attributing spend events to advertisment impressions with mapreduce  

* Finalist TAG 2015 Mobility live [hack-back](http://www.hubga.com/tag-press-release/finalists-revealed-for-mobility-live-hack-back-invitational/) - Dichotomous key for entomology education  

* Various open source contributions. Check out my [github](https://github.com/chrisevett)  


### Education  
BS Biology major Math minor, University of West Georgia 2009  
Graduate coursework in Biology, Georgia Southern University 2011-2013  
Coursework in Computer Science, Oregon State University 2015  