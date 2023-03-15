
<h1>Active Directory: Joining a Windows 11 PC to a domain</h1>



<h2>Description</h2>
For this Lab, we will add a Help Desk Computer to the domain. One important thing to note is that Help Desk personnel will have access to things other in your organization may not. For example, they may have access to Active Directory, but not complete access to Windows Server, while a normal user will not have access to either. Help Desk computers should have their Administrator account enabled on their computer.  In this lab our domain is ReggieTech.comand the PC name is Desktop2ADlab
<br />




<h2>Environments Used </h2>

- <b>Windows 11 Pro  **Note: You cannot add Windows Home PCs to a Domain**</b> 

<h2> Adding a Windows 11 PC to a domain </h2>

<p align="center">
Notice, at the sign in screen we only have an option for the administrator. This is because the other user accounts on the PC are disabled, and we are not joined to a domain.<br/>
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%201.png"/>
<br />


<br />
Since we know this will be a Help Desk user, we can go ahead and give the user access to some of the Roles and Features that the Windows Server Manger would have. Remember, they won’t have access to everything, just what is needed for their role.  We will start by going to Optional Features. This can be done by typing optional features in the search bar. Once you are there, just select view features.<br/>
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%202.png"/>
<br />


<br />
Now you will have the option to scroll down and see all the available features. As you scroll, you’ll start to see RSAT features/tool. These are the features/tools you would want to install on your help desk computer. Your organization would determine which features/tools a user would have access to. For this lab we will give the user access to quite a few features/tools. DNS management tool, DHCP management tools, Server management tools, Domain system, and remote access to name a few. Once all the features/tools are selected, hit next and install. (**Note: RSAT features and tools allow you have services on an non Windows Server PC.) <br/>
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%203.png"/>
<br />


<br />
Now all tools are installed, we are all set right?? Not quite, keep in mind, we are still not joined to a domain, so none of the tools will work. <br/>
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%204%20pt%201.png"/>
<br />


<br />
To join the PC to a domain we will double click File Explorer from the home screen and right click on properties.  <br/>
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%205%20pt%201.png"/>
<br />



  <br />
Next you will scroll down to related links and select Domain or workgroup. <br/>
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%206.png"/>
<br />


<br />
Select to rename this computer or change its domain or workgroup, click change. Go to the Member of section and type in the domain name you wish to join. You should receive a message that says welcome to the domain and a message asking you to restart your PC. <br/>
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%206.png"/>
<br />
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%206.png"/>
<br />
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%206.png"/>
<br />



<br />
After you restart, you will notice that you have the option to sign into your Domain. Now you can sign in with an account in your domain to this PC. You can also verify by going to the Server Manager and looking in Computers under your domain name. In this lab, you see my PC (Desktop2ADlab) under the ReggieTech Domain.  <br/>
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%206.png"/>
<br />
<br/>
<img src="https://github.com/Rastallworth1/Enabling-an-Administrator-account-on-Windows-11/blob/main/Screenshot%206.png"/>
<br />




 
  
  


<br />
This was a simple Active Directory Home Lab / Tutorial thats demonstrates the proper steps to enable an Administrator account on a Windows 11 PC.<br/>
