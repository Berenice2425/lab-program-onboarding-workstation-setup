# Program Onboarding & Workstation Setup

📘 Hands-on project from SKILL.SCH CloudLabs.

Create Your Workspace and Git Repository
Create a dedicated folder for this lab that is your workspace, turn it into a Git repository on the main branch, and make a first commit with a README and a .gitignore

<img width="405" height="86" alt="{FE4495EA-2787-40C6-8445-EAB4266932B3}" src="https://github.com/user-attachments/assets/a46652d3-3eda-43a3-ab60-106dc428d749" />

This step makes a folder for the lab with mkdir -p (which creates parent folders as needed and does not fail if the folder exists) and moves into it with cd.


<img width="418" height="108" alt="{B6239124-288A-4298-BFBC-6921078D1B5B}" src="https://github.com/user-attachments/assets/4b85c411-3a8c-48ac-b1c3-ffcad1da3b4a" />

git init -b main turns the folder into a repository whose first branch is called main.
 
<img width="411" height="78" alt="{E9C0094F-33AE-44D9-B148-560FDA066CB6}" src="https://github.com/user-attachments/assets/fc4cab39-7bef-4a81-857b-2ec6fcca5b7f" />

<img width="425" height="161" alt="{57A951D5-28E6-4676-8072-4180A7E64DA2}" src="https://github.com/user-attachments/assets/016ed7df-06ee-4f09-b6bc-9f6a8113a1f1" />

The two printf lines write a short README.md and a .gitignore listing files Git should never track, such as node_modules, .env secrets and Terraform state.
 
<img width="430" height="164" alt="{975A6A48-1EB5-4736-9C3C-EB54B428D601}" src="https://github.com/user-attachments/assets/ba421b53-49b7-485d-a5a2-f8bfac0ad108" />

 git add stages both files and git commit saves them as the first snapshot with a descriptive message.


💡 Git is a version control tool that records snapshots of your files so you can track and share your work. 
Every real engineering task starts in version control. Working in one repository lets you commit after each mission and push the finished project to GitHub as portfolio evidence.

📘 Verify Workstation RAM & OS Readiness.

Check how much RAM your machine really has so you can confirm it meets the 8 GB minimum.
Requirement: computer with 8 GB RAM minimum (Windows or macOS both work)
  - Linux / WSL:
free -h

 - macOS (prints bytes; 8 GB = 8589934592):
sysctl -n hw.memsize

 - Windows PowerShell:
 (Get-CimInstance Win32_ComputerSystem).TotalPhysicalMemory / 1GB


Labs, browsers, terminals and containers run more smoothly with at least 8 GB of RAM. Instead of just printing a message, this step reads the real total memory: on Linux or WSL, free -h shows memory in human-readable units; on macOS, sysctl -n hw.memsize prints it in bytes; on Windows PowerShell, Get-CimInstance Win32_ComputerSystem reports TotalPhysicalMemory. Compare the result with the 8 GB minimum. Windows or macOS are both fine for the course.~~~

📘Create Your Azure Free Trial Account.

Provisions your personal Microsoft Azure subscription with $200 in free credit for 30 days.
Azure is Microsoft's cloud platform, and a free account gives new users a credit (USD 200 at the time of writing) to spend within 30 days, plus some services free for 12 months. You sign up at azure.microsoft.com/free with a Microsoft account and verify with a phone number and card, which is used for identity checks rather than charged. Afterwards check the credit in the Azure portal under Cost Management or Subscriptions.
You will use the Azure Portal and Azure CLI throughout the program to deploy real cloud resources.

📘Set Up Your Dev.to Account for Assignments.
<img width="646" height="179" alt="{10F214AA-6DC0-4B3D-8D9C-9BC29B93E940}" src="https://github.com/user-attachments/assets/4c485ce3-cde3-4404-a604-61cf49bebdfd" />

Establishe your public developer blog on Dev.to where you will publish your program assignments.

Dev.to is a free blogging platform for developers where you will publish your written assignments. Create an account at dev.to, then fill in your name, photo and short bio so your posts look professional. Hashnode or Medium are accepted alternatives, but you only need one.

📘Create Your Professional GitHub Account.

<img width="662" height="386" alt="{B3645F41-C0E9-400B-9F86-82A10E9F2104}" src="https://github.com/user-attachments/assets/19a3b370-10aa-412d-ab3a-4d6206cf314b" />

Set up your professional GitHub identity for code repositories while keeping Dev.to as your publishing home for written articles.
GitHub hosts Git repositories and will be your public portfolio of code. Sign up at github.com, choose a professional username, verify your email address and add a profile photo.

<img width="627" height="186" alt="{EABAF07B-50D4-4A9E-BF61-072A2D8D0893}" src="https://github.com/user-attachments/assets/a683e899-3485-4c78-b0b3-7ef05f493f96" />

<img width="429" height="252" alt="{A7D3BD21-C80B-4677-B65C-FEA08A5E030D}" src="https://github.com/user-attachments/assets/5592a378-4446-494d-b87d-3ea4280ae476" />

<img width="415" height="85" alt="{F0BC313F-B1B2-428B-A31E-CE8D668747B1}" src="https://github.com/user-attachments/assets/1d575586-6d86-44fa-b0dd-a79ff27a19d4" />


Your code goes on GitHub while your written articles stay on Dev.to. Recruiters review both your GitHub handle (for code) and your Dev.to blog (for technical articles).
