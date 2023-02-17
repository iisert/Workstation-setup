# Workstation-setup
This repo contains all the modifications done on the latest pc for the Complex networks and dynamics group at IISER Tirupati.

***

# Instruction Set:
1. Installed OpenSSH Server and Client using https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell
2. Created users and added them to administrators group using https://support.microsoft.com/en-us/windows/create-a-local-user-or-administrator-account-in-windows-20de74e0-ac7f-3502-a866-32915af2a34d
3. Installed Tailscale VPN to access PC using machine names.
  i. Signed up using the complexnetworksanddynamics@gmail.com
  ii. Created a windows service for the app to remove restriction of logon after reboot using http://runasservice.com/
4. Installed Python on system using https://www.python.org/downloads/
5. Installed required packages like jupyterlab, matplotlib, pandas, numpy,... using pip
6. 

# How to use HP Z2 G9 Workstation remotely:
1. Create your user/pass on the workstation.
2. Install SSH Client on your local machine. 
3. Install Tailscale on your local machine.
4. Sign in using the group Gmail id and pass.
5. Connect using the command: 
'''
$ ssh (user)@workstation
'''
6. You are now in the workstations terminal

# How to use HP Z2 G9 Workstation for Jupyterlab/notebook remotely:
1. SSH into the Workstation using the above guide
2. Use **1.** of https://docs.anaconda.com/anaconda/user-guide/tasks/remote-jupyter-notebook/ to run jupyter notebook 
3. Open a new terminal window, without closing the previous one, and proceed to step 2 of above link.
4. This has created a SSH Tunnel to the remote server. Now copy paste the link from step 1 in the browser of the local machine.
5. Another guide for the same: https://towardsdatascience.com/connecting-to-a-jupyter-notebook-on-a-remote-linux-machine-277cef04abb7
