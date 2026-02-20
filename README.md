# DevOps_webapp
End-to-End DevOps Automation Using CI/CD, ChatOps & Static Deployment

#Overview
This project demonstrates a complete DevOps automation workflow using GitHub Actions for Continuous Integration (CI), Slack for ChatOps notifications, and Netlify for Continuous Deployment (CD). The objective is to automate build, notification, and deployment of a static web application whenever code is pushed to the main branch.

Technologies Used
Git and GitHub
GitHub Actions
Slack Incoming Webhooks
Netlify
HTML

Workflow
When code is pushed to the main branch, GitHub Actions automatically triggers the CI pipeline. The workflow checks out the repository and executes build steps. After successful execution, a Slack notification is sent to the configured channel. Netlify, connected to the GitHub repository, automatically deploys the updated version of the website. The live URL reflects changes without any manual intervention.

Continuous Integration
The CI pipeline is configured using a YAML file inside the .github/workflows directory. It runs automatically on every push to the main branch and displays build logs and execution status.

ChatOps Integration
A Slack Incoming Webhook is configured and stored securely as a GitHub repository secret. The pipeline sends automated build status notifications to the Slack channel after execution.
<img width="1915" height="818" alt="Screenshot 2026-02-20 192209" src="https://github.com/user-attachments/assets/2e986164-0f47-427e-93cf-65c77beb3b27" />


Continuous Deployment
The GitHub repository is connected to Netlify using the “Import from Git” option. Auto-deploy is enabled on commits to the main branch. Every successful push triggers automatic build and deployment.

<img width="1872" height="881" alt="Screenshot 2026-02-20 192412" src="https://github.com/user-attachments/assets/28f8ae00-a1a3-431d-8e71-98539fa8af5f" />

Testing Automation
To verify automation, changes are made to index.html and pushed to the main branch. The CI pipeline runs automatically, Slack receives a notification, Netlify triggers a deployment, and the live website updates accordingly.

<img width="1359" height="729" alt="Screenshot 2026-02-20 191926" src="https://github.com/user-attachments/assets/00172ee4-6fec-49e0-afc6-16d8a81df697" />
<img width="1918" height="949" alt="Screenshot 2026-02-20 192104" src="https://github.com/user-attachments/assets/d56c2467-134e-497a-bb0a-aadb9f295ec5" />


Conclusion
This project successfully implements an end-to-end DevOps pipeline integrating CI, CD, and ChatOps. 
It demonstrates automated build, notification, and deployment processes aligned with real-world DevOps practices.
