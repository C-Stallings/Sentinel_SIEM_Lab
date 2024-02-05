<h1>WORLD MAP FAILED RDP HONEYPOT</h1>

<h2>Description</h2>
<b>Developed a honeypot on a virtual machine to perform the following tasks for Microsoft Azure Sentinel (SIEM)
</b>
<br />
<br />
The Powershell script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot.
Live, global attacks were observed, recorded and plotted in Microsoft Azure Sentinel Map using Geolocation information.
<br />
<br />


<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>LogExporter running PowerShell script from Window Event Viewer</h2>

<p align="center">
<img src="https://github.com/C-Stallings/Sentinel_SIEM_Lab/assets/61432825/38787586-98aa-4844-9614-5ab1c2dbb623" height="85%" width="85%" alt="LogExporter_screenshot"/>
</p>

<h2>Per the logs, attacks are currently coming to the Windows virtual machine from Peru based on the geodata. Utilizing ipgeolocation.io, the geodata will be plotted in Microsoft Sentinel</h2>

<p align="center">
<img src="https://github.com/C-Stallings/Sentinel_SIEM_Lab/assets/61432825/c623a75b-8db6-417b-a3f1-348ebc9ce07d" height="85%" width="85%" alt="LogExporter_screenshot">
</p>

<h2>World map of the incoming attacks after ~6-8 hours built with a custom log to include the geodata. Below will show the attacks were coming from source network addresses in Germany, Peru and Russia</h2>


<p align="center">
<img src="https://github.com/C-Stallings/Sentinel_SIEM_Lab/assets/61432825/db328b10-091d-4286-bf08-758f878d2968" height="85%" width="85%" alt="World_Map_Failed_RDP_screenshot"/>
</p>
