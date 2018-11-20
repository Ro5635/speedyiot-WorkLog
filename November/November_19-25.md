## 19th November

Today I setup the work log, all progress in the project will now be recorded in this log book. I have used the docsify tool to do this as it allows me to write the log files in markdown and have these viewable in a web format.

This has been deployed to a subdomain of my personal site, there is no authentication details required to access this log. I am using this system in preference to using a hand written physical log book, this is due in part to my near ineligible hand writing and preference for a system where the content can be reliably backed up.

The log book has been deployed as a serveries service, it is hosted on S3 and Cloud Front. These are the block storage and content delivery services of AWS. This redeploys on a commit to the master branch of the work log GitHub repository, this is managed by a deployment pipeline that is configured on AWS to listen for a web hook from GitHub and then trigger a build process that copy's the latest updates to S3 and then clears the Cloud Front cache.

### SpeedyIOT  Web App

I have also created the repository and an empty Angular application for the project web app, this is configured so that all of the usage of the Angualr API and builds are carried out within a docker container, this is advantageous as it removes any requirement that the host machine is set in any state other than able to run Docker, this reduces the risks that issues will occur later in the project with the build chain that blocks progress.

## 20th November

### SpeedyIOT  Web App 

Today I deployed the infrastructure that is required to host the web app and website for the project. This was compleated on my project AWS account.

## 21th November
