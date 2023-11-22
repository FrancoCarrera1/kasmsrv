# Kasm Server
This is a repository outlining how I setup a Kasm server, and why I set it up.

## Why Kasm?
<br> For many of us IT professionals out there who are just starting to learn, Kasm was the most cost effective solution for me to be able to launch VM's at will for virtually free since it takes advantage of docker containers to do this. With this you can launch docker containers that can run any OS out there. I will mainly be using this to educate myself on Linux and Networking further.
- [<b>All original Kasm documentation can be found here:](https://kasmweb.com/docs/latest/install/single_server_install.html)

<h1>Prerequisites for Kasm.</h1>
<ul>
<li>Ubuntu or any of the supported operating systems</li>
<li>2  Core CPU, 4GB RAM, 50GB(SSD preferred)</li> (I personally used an old HP Mini DT)
</ul>

<h2>Installing Kasm</h2>
The first thing we want to do is cd (change directory) on our linux machines, we do that using the cd command followed by the directory we want to go to. In our case want to go to the temp directory and we will do this using cd /tmp.
<img src="https://github.com/FrancoCarrera1/kasmsrv/blob/main/images/cdcmd.png" height="80%" width="80%" alt="kasmcd"/>

Then we use the curl command to download Kasm from the official website <b>"curl -O https://kasm-static-content.s3.amazonaws.com/kasm_release_1.14.0.3a7abb.tar.gz

<img src="https://github.com/FrancoCarrera1/kasmsrv/blob/main/images/curlkasm.png" height="80%" width="80%" alt="kasm curl"/>

After that is done downloading we must exract the file we just downloaded and we do that using <b>"tar -xf kasm_release_1.14.0.3a7abb.tar.gz

<img src="https://github.com/FrancoCarrera1/kasmsrv/blob/main/images/tarcmd.png" height="80%" width="80%" alt="tarcmd"/>

Finally we use the "sudo bash kasm_release/install.sh" which gives us superuser permissions to install Kasm on the computer. After this command the installation may take awhile

<h3>Post-Installation Steps</h3>
At the end of the installation, you will receive text with your Kasm UI Credentials. The username will be admin@kasm.local, and the password will be below it. It will look like the following
<img src="https://github.com/FrancoCarrera1/kasmsrv/blob/main/images/ksmcred.png" height="80%" width="80%" alt="tarcmd"/>

After this you can use the "ifconfig" command to find the ip of the server, a tip I can give to Make this easier which is something I did, is to logon to your DHCP Server, for many of you at home that requires logging into your ISP's router. And many of them will have a feature that will let you set the device that is hosting Kasm to a static ip. All you need is the MAC address of the device that you are using and matching it on your routers end to set the ip statically. After that is done open up a web browser, type in the https://(ip goes here). And you will be at the webpage asking for credentials
<img src="https://github.com/FrancoCarrera1/kasmsrv/blob/main/images/kasmstart.png" height="100%" width="100%" alt="logon screen"/>

Login with your credentials, and make sure you change that default password for Security. After that I recommend you use the Kasm Documentation to learn the platform, and how you can launch containters with various os like Kali, Parrot, Postman, and even text editors and web browsers! There is also a Chrome extension that lets you open links you may think are suspicious in one of these containers. 





