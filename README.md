# Continuous-delivery-using-jenkins
Continuous delivery of java web app using jenkins and tools

### 
This project is a step to step procedure of continuous delivery with jenkins and other tools. I had previously written an a step to step procedure on continuous integration.

The solution to manual code deployment is to:
. Build, test, deploy and test for every commit
. Automated process
. Notify for every build status
. Fix code if bugs or error found instantly rather than waiting.

### TOOLS
. Jenkins
. Git (version control system)
. Maven
. Checkstyle (Code analysis tool)
. Slack (Notification)
. Nexus (Artifact/software repository)
. Sonarqube (Code analysis server)
. Apache tomcat (Java web application server)
. Selenium (Software testing)
. Windows server (Slave of jenkins for software test suit)
. AWS (EC2 instances for all the servers)

### OBJECTIVES
. Fault isolation
. Fast turn around on features changes (means any new request or new code change, it can be built quickly by the developer and delivered quickly)

### FLOW OF EXECUTION FOR CONTINUOUS DELIVERY AFTER RUNNING CONTINUOUS INTEGRATION JOB:
.Create Security group: (a) Windows server (b) Tomcat and backend servers
. Setup tomcat and backend server on EC2 with userdata
. Create Jenkins job to deploy artifact to staging.
. Add windows node as slave to jenkins
. Create job to run software test(Selenium) from windows server
. Deploy artifact to production tomcat server
. Connect all the jibs with build pipeline
. Test it by committing code to github.


