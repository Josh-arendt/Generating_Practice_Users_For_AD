Generating Practice Users for Active Directory. 
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Generating Practice Users for Active Directory.</h1>
This step-by-step guide details the proccess of using a PowerShell script to generate "dummy" user accounts within Active Directory. 
This tutorial is for users who wish to experiment and practice with Active Directory 
*Assumes the steps covered in the previous repositories have already been implemented.*
<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop
- Active Directory Domain Services
- PowerShell
- Personal Computer


<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Broad Concepts </h2>

- Step 1 Generate practice users with a PowerShell script.
- Step 2 Observe Users being created. 
- Step 3 Practice logging in as one of the generated Users.  

<h2>Detalied Deployment and Configuration Steps</h2>

<p>
  
  ![image](https://github.com/Josh-arendt/Generating_Practice_Users_For_AD/assets/140751318/00161aa3-076b-4d52-9bee-44678943e8a5)
 
</p>
<p>
Inside the domain controller, run PowerShell ISE as administrator.
<br />

<p>
  
  ![image](https://github.com/Josh-arendt/Generating_Practice_Users_For_AD/assets/140751318/eb7f15ee-86da-41ab-ac4f-8af0ee7917da)

</p>
<p>
In the top-left corner, select "New Script." copy and paste the following script into PowerShell ISE: 
  
  [PowerShell Script](https://github.com/Josh-arendt/Generating_Practice_Users_For_AD/blob/main/PowerShell%20Script.txt)
  
Select "Run Script".
-Feel free to adjust the number of users you would like to generate. 10,000 users is a little too much for this example. 
-Please take note of which file the users are being dumped into. for this tutorial, the script is putting Users into the folder labled "_EMPLOYEES." Make sure the name of the folder in the script matches the name in the direcotry.  
<br />

<p>
  
  ![image](https://github.com/Josh-arendt/Generating_Practice_Users_For_AD/assets/140751318/1686cc34-e9f4-4423-9604-6381a433f721)
 
</p>
<p>
Observe the generated users in the "_EMPLOYEES" folder. 
At this point, you may practice assigning some Users to different security goups. You may also want to practice assigning different permissions to some users. 
<br />

<p>
  
  ![image](https://github.com/Josh-arendt/Generating_Practice_Users_For_AD/assets/140751318/2a36f6f9-1db1-4be0-954a-455402682a36)

</p>
<p>
Select one user and practice logging in as them on the Client PC. The usernames you have generated will be different than the ones in this example since they are generated randomly.
(If you copied the PowerShell script, the password will be "Password1" for this example.) 
<br />

<p>
  
  ![image](https://github.com/Josh-arendt/Generating_Practice_Users_For_AD/assets/140751318/e2bd9b04-e804-4587-a254-ce1922925df7)

</p>
<p>
Success!! All of your generated Domain Users can log into the Client PC!
<br />
