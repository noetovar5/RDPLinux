# RDPLinux          <img align="right" src="https://visitor-badge.laobi.icu/badge?page_id=noetovar5.RDPLinux"/> 
set up rdp for your kali linux vm


#Use remote Desktop Protocol (RDP) to connect to a Kali Linux virtual machine (VM) from a Windows computer by following these steps:

Step 1: Enable RDP on Kali Linux:
- Install the xrdp package on your Kali Linux VM by running the command:
  ```
  sudo apt update
  sudo apt install xrdp
  ```
- Start the xrdp service:
  ```
  sudo service xrdp start
  ```

Step 2: Configure Firewall (if needed):
- Allow traffic on port 3389 (default RDP port) through the firewall on your Kali Linux VM if it's enabled:
  ```
  sudo ufw allow 3389/tcp
  ```

Step 3: Obtain Kali Linux VM's IP Address:
- Find the IP address of your Kali Linux VM by using the `ifconfig` command:
  ```
  ifconfig
  ```
  Look for the IP address under the appropriate network interface (e.g., eth0, wlan0).

Step 4: Connect from Windows using Remote Desktop Connection:
- On your Windows computer, open the Remote Desktop Connection application. You can do this by searching for "Remote Desktop Connection" in the Start menu.
- Enter the IP address of your Kali Linux VM in the "Computer" field.
- Click "Connect," and if prompted, enter the username and password for your Kali Linux VM.

Step 5: Access Kali Linux via RDP:
- Once connected, you'll have remote access to your Kali Linux VM from your Windows machine using the Remote Desktop Connection.

Please note:
- Make sure your Kali Linux VM and Windows computer are on the same network or have proper network connectivity.
- Ensure that your Kali Linux VM is up to date and has the xrdp package installed.
- If you encounter any issues connecting, double-check firewall settings, network configurations, and any potential conflicts with RDP ports or security settings.

This method should enable you to establish an RDP connection to your Kali Linux VM from your Windows system for remote access.
