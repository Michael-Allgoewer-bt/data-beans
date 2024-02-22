# Data-Beans-Demo

Welcome to Data Beans, a fiticous company that has a fleet of coffee trucks located in cities around the world.  The source code provided here is design to high how you can use GenAI along with BigQuery on Google Cloud.  The code is all working and was used to construct the demo.  The demo consists of a web frontend along with the backend code contained in the project.  To see the frontend, currently is it not deployed as part of the demo, please contact your account team or customer engienner.

This demo is an end to end working demo with all code provided so you can use based upon the contained license agreement.

## Data Generation
- All data in this demo is synthetically generated by LLMs.  
- All images in this demo are generated by GenAI.

## How to deploy
The are two options to deploy the demo depending on your access privilages to your cloud organization

# ALERT
# This is still being tested due to some recent changes!

### To deploy to New Project (Requires Elevated Privileges)
- **The following IAM roles are required to deploy the solution**
   - Prerequisite:  Billing Account User (to create the project with billing)
   - Prerequisite:  Organization Administrator (to create all assets)
   - Optional:      Folder Editor (if you alter the script to place the project in a folder)
1. Open a Google Cloud Shell: http://shell.cloud.google.com/
2. Type: ```git clone https://github.com/GoogleCloudPlatform/data-beans```
3. Switch the prompt to the directory: ```cd data-beans```
4. Run the deployment script: ```source deploy.sh```
5. Authorize the login (a popup will appear)
6. Follow the prompts: Answer “Yes” for the Terraform approval.


### To deploy to an Existing Project (Requires Assistance from IT and Owner Project Privileges)
- **The following items are required to deploy the solution**
   - Prerequisite: You will need a project created for you (IT can do this for you)
   - Prerequisite: You will need to be an Owner (IAM role) of the project to run the below script
1. Open a Google Cloud Shell: http://shell.cloud.google.com/
2. Type: ```git clone https://github.com/GoogleCloudPlatform/data-beans```
3. Switch the prompt to the directory: ```cd data-beans```
4. Update the hard coded values in ```deploy-use-existing-project-non-org-admin.sh```
5. Run ```source deploy-use-existing-project-non-org-admin.sh```

