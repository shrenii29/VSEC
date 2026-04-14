# Assignment 8

a. Create a repository on GitHub and upload project files.  
b. Install and launch Jenkins (http://localhost:8080).  
c. Install required plugins (Git, GitHub, Pipeline).  
d. Create a new Pipeline job in Jenkins.  
e. Configure Pipeline script from SCM and add GitHub repository URL.  
f. Add a Jenkinsfile to the repository.  
g. Configure build trigger (Poll SCM or GitHub Webhook).  
h. Push code changes to GitHub.  
i. Verify that Jenkins automatically triggers the build.

- Install jenkins.war file. Put it in a folder VSEC/jenkins
- Install java 17 or 21 from oracle
- open cmd from the folder containing jenkins.war file
- use the command: ``` java -jar jenkins.war httpPort=8080 ```
- after installation, open http://localhost:8080 and complete initial setup
- if plugins are not installing, skip forward. click on **Start using jenkins**

###  Step 1: Fix the Update Center URL first

- Click "Manage Jenkins" on the left sidebar
- Click "Plugins"
- Click "Advanced settings" tab at the top
- Scroll down to "Update Site" section
- Clear the existing URL and replace it with:

   ```https://updates.jenkins.io/update-center.json```

- Click "Submit"

### Step 2: Refresh the plugin list

- Click "Available plugins" tab
- Click "Check now" button (bottom right)
- Wait 30 seconds, then refresh the page

### Step 3: Download the required Plugings

- git
- github
- pipeline

