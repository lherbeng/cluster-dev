
# **How to use Jenkins in wsl2 Ubuntu to build a pipeline for the development of the Rancher RMS cluster**

***Prerequisites:***

- Make sure you have WSL 2 and Ubuntu installed on your Windows machine.
- Rancher Desktop should be installed and running.
- VS Code should be installed with the necessary extensions for Docker, Kubernetes, and Jenkins.

***Step 1: Install Jenkins in WSL 2***

You can install Jenkins in WSL 2 by running the script jenkinsinstallation.sh

![image](https://github.com/lherbeng/cluster-dev/assets/72662912/19d46ea6-d33b-4245-ba12-c8d6b5dd26c8

Jenkins should now be installed and running in your WSL 2 Ubuntu instance. Access the Jenkins web interface by opening your web browser and navigating to http://localhost:8080. Follow the setup wizard to complete the Jenkins installation.

***Step 2: Install Jenkins Plugins***

After Jenkins is installed, install the necessary plugins for Rancher, Docker, and Kubernetes. You'll need these plugins to create a pipeline that interacts with your Rancher RKE cluster.

1. Go to the Jenkins dashboard (usually at http://localhost:8080).
2. Click on "Manage Jenkins" > "Manage Plugins" > "Available."
3. Search for and install the following plugins:
   
- Kubernetes
- Docker Pipeline
- Rancher

