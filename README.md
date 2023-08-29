
# **How to use Jenkins in wsl2 Ubuntu to build a pipeline for the development of the Rancher RMS cluster**

***Prerequisites:***

- Make sure you have WSL 2 and Ubuntu installed on your Windows machine.
- Rancher Desktop should be installed and running.
- VS Code should be installed with the necessary extensions for Docker, Kubernetes, and Jenkins.

***Step 1: Install Jenkins in WSL 2***

You can install Jenkins in WSL 2 by running the script jenkinsinstallation.sh

![image](https://github.com/lherbeng/cluster-dev/assets/72662912/1e17ddbb-2399-4cbd-b140-781a195b093b)


Jenkins should now be installed and running in your WSL 2 Ubuntu instance. Access the Jenkins web interface by opening your web browser and navigating to http://localhost:8080. Follow the setup wizard to complete the Jenkins installation.

***Step 2: Install Jenkins Plugins***

After Jenkins is installed, install the necessary plugins for Rancher, Docker, and Kubernetes. You'll need these plugins to create a pipeline that interacts with your Rancher RKE cluster.

1. Go to the Jenkins dashboard (usually at http://localhost:8080).

![image](https://github.com/lherbeng/cluster-dev/assets/72662912/a62e095c-d6da-4081-a1cd-5b52d5c06d05)

2. Click on "Manage Jenkins" > "Manage Plugins" > "Available."
3. Search for and install the following plugins:
   
- Kubernetes
- Docker Pipeline
- Rancher

4. Validating a Jenkinsfile using Visual Studio Code can be done using the "Jenkins Pipeline Linter Connector" extension. This extension allows you to lint (validate) your Jenkinsfile directly within Visual Studio Code, providing instant feedback on any syntax errors or issues. Here's how you can set it up and use it:

- Install Visual Studio Code: If you haven't already, download and install Visual Studio Code from the official website.

5. Install Jenkins Pipeline Linter Connector Extension:

![image](https://github.com/lherbeng/cluster-dev/assets/72662912/10663d46-f179-47d3-b9b5-7640f1becbcf)


- Open Visual Studio Code.
- Click on the Extensions icon in the sidebar (or press Ctrl+Shift+X on Windows/Linux or Cmd+Shift+X on macOS).
- Search for "Jenkins Pipeline Linter Connector" and click "Install" for the official extension developed by Microsoft.
