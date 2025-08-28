<p align="center">
<img src="" alt=""/>
</p>

<h1>Setting Up Tailscale VPN on Home Lab</h1>
This tutorial outlines the  installation of Tailscale on my Home Lab<br />



<h2>Environments and Technologies Used</h2>

- VPN
- CLI
- Tailscale


<h2>Operating Systems</h2>

- Linux
- Proxmox


<h2>Installation Steps</h2>

<p>
1. First I installed proxmox to my home server
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/0d444471-95bc-461e-b6f5-9f9cdd242141" height="80%" width="80%"/>
</p>
<br />



<p>
2. Next I used this install script given in the tailscale setup to install tailscale on the main pve node shell
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/0123de93-4d3b-453a-92df-0c987835bd13" height="80%" width="80%"/>
</p>
<br />


<p>
3. Next I need to make a tailscale account
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/56ba3a33-b0db-40c5-bf5f-5b93591fa4f5" height="80%" width="80%"/>
</p>
<br />

<p>
4. Next I added my server to the tailscale account using the script given in the add devices dropdown.  After that i downloaded tailscale on my main computer and my phone
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/519655df-3e4d-4afc-8cdf-a2fdf0666c09" height="80%" width="80%"/>
</p>
<br />

<p>
5. Now on my main PC I started tailscale using sudo tailscale up, then I SSH'd into the server using ssh root@pve
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/5c5084b0-d593-48d9-a3ab-95c9e65d23ce" height="80%" width="80%"/>
</p>
<br />

<p>
6. Lastly to avoid SSL and certificate annoyances when logging in through https, I then installed tailscale serve on the server to automatically create and sign certificates
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/50dc856b-3468-4026-bcf6-dbd2f34103aa" height="80%" width="80%"/>
</p>
<br />
