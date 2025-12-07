**📦 Project 1 – Part B: Docker Image Build, ECR Push & Final Deployment (Jenkins + Ansible + AWS)**

**This repository represents Part B of the full CI/CD lifecycle project.
While Part A covered planning, CI setup, Terraform provisioning, and Ansible configuration, Part B focuses on the final deployment stages:**

 🔵 Docker Image Build.
 
 🔵 Push to AWS ECR.
 
 🔵 Jenkins CI/CD Pipeline Execution.
 
 🔵 Deployment to EC2 (Ansible).
 
 🔵 Final Verification & Closure.


**🛠️ Tools & Technologies Used**

🔵 CI/CD:	Jenkins, GitHub

🔵 Containerization:	Docker

🔵 Cloud:	AWS EC2, ECR

🔵 Project Tracking: Jira, Slack


🚀 Project Workflow:
** Deployment and Documentation**

1. **Push Docker Image to ECR**
   - Tag and push your Docker image to AWS ECR.
     
   - Ensure Jenkins pipeline pulls the image from ECR for deployment.

2. **Deploy App to EC2/ECS**
   - Final deployment using Jenkins/Ansible.
     
   - Access the app in browser using EC2 public IP or load balancer.

3. **Update Jira Ticket**
   - Move task to "Done" or "Resolved".
     
   - Add a summary comment: what you did, links to repo, any blockers.

4. **Send Slack Message**
   
   - Inform your team: "Deployment complete. jira updated."

**How to run the project:**

6️⃣ Build & Push Application Image

•	Build the Docker image of the application.

•	Push the image to AWS ECR so Jenkins can pull it during deployment.

•	Verify that the image is available in the ECR repository.

________________________________________
7️⃣ Execute Full Jenkins Pipeline

•	Trigger the Jenkins pipeline or let it trigger automatically via GitHub webhook.

•	The pipeline will:
o	Pull the latest code
o	Build and package the application
o	Push the Docker image to ECR
o	Deploy it to the configured EC2 instance using Ansible

•	Monitor each stage from the Jenkins dashboard.

________________________________________
8️⃣ Access the Deployed Application

•	Once deployment succeeds, open the application in your browser using:
EC2 Public IP or Load Balancer URL

•	Confirm the application is running as expected.
________________________________________
9️⃣ Close the Project

•	Mark the Jira ticket as Resolved/Done.

•	Leave a comment summarizing the work completed.

•	Notify the team on Slack

**📸 Screenshots:**

 🔵 Installed AWS, Docker, Jenkins on a new EC2:

  <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/b9898dd0-a4af-435c-a259-b64590d847cb" />

 🔵 Jenkins pipeline sucess:

  <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/c1e7a9f4-0e90-49a3-a376-227ff9645bb0" />

 🔵 ECR Image Pushed:
 
 <img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/89c8f6a4-a10f-4756-b3c2-4380c26e25b8" />

 🔵 EC2 Deployment:

 <img width="941" height="456" alt="image" src="https://github.com/user-attachments/assets/29ae6a2b-9e38-4de9-8b45-974ad97189b3" />

 🔵 Application Running via EC2 public IP and ALB dns:

 <img width="944" height="230" alt="image" src="https://github.com/user-attachments/assets/e594374e-b759-41dd-9504-8f46b7f7fbea" />

 <img width="944" height="238" alt="image" src="https://github.com/user-attachments/assets/4da5de90-9fd0-403f-b050-cc72bd683fc3" />

🔵**Conclusion**
Part B completes the final deployment stage of the CI/CD pipeline. 
This includes building and pushing the Docker image to ECR, executing the Jenkins pipeline, and deploying the application to an EC2 instance using Ansible.

Together, Part A and Part B demonstrate a complete end-to-end DevOps workflow — from planning to infrastructure provisioning to final production deployment.




 




