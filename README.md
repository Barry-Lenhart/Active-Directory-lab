# Basic Home Lab Running Active Directory

This repository contains steps on how i set up a basic home lab running Active Directory following a tutorial by [Josh Madakor](https://www.youtube.com/@JoshMadakor)

## Diagram
![Diagram](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/3c316a95-fbf2-420a-874a-a842773e05ca)
)

## Download and install Oracle VirtualBox from the official website.
[Oracle Virtual Box](https://www.virtualbox.org/)

## Download the Windows 10 and Server 2019 ISO files.
[Windows 10 iso](https://www.microsoft.com/en-us/software-download/windows10ISO)
[Windows Server 2019](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

## Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller," and selecting the "Windows Server 2019" ISO file as the boot media.

![Pasted image 20230402145533](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/dade37ba-e2ea-4c0b-8ce5-5010cd3f808d)



![Pasted image 20230402145610](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/0e778d29-1c1a-4d9f-9cf4-afb1b0547099)


##  Configure the virtual machine by giving it two network adapters: one for connecting to the internet and the other for the private network.

![Pasted image 20230402145806](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/b454594f-7734-4b88-8a28-3511ab00061e)


![Pasted image 20230402145820](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/aa6fb448-5a18-46cf-9240-bc5c2e03cac9)


##  Install Server 2019 on the virtual machine and assign IP addressing for the internal network.

![Pasted image 20230402150458](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/889eb9db-6f32-405d-898e-1374c5097fa1)


![Pasted image 20230402150538](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/06d34509-0d80-412b-95c9-950d6fa05f1a)

##  Name the server and install Active Directory to create the domain.
![Pasted image 20230402150727](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/6431f5c9-6d5b-48b7-b94e-fd510494b5b6)


![Pasted image 20230402153253](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/98e71a41-6393-4091-9037-d8cf67ed7fb3)


##  Configure routing so that clients on the private network can access the internet through the domain controller.

![Pasted image 20230402153829](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/2aa8239b-a9cb-4b54-bfc9-c803b4922703)


![Pasted image 20230402153904](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/de92b308-606d-4198-8dd8-56ee91bcd26b)


![Pasted image 20230402154123](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/568c0a70-7d33-435f-b2ac-aeafc02115b2)


##  Set up DHCP on the domain controller.

![Pasted image 20230402154312](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/38c7f9bb-9952-4bee-a8a4-072998fc4db8)


![Pasted image 20230402154041](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/495d9c51-dadf-4f21-9b92-98f221712a4f)


![Pasted image 20230402154439](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/db488d20-b3e8-4c72-b16b-8567fb01789d)



##  Run the PowerShell script to create 1000 users in Active Directory.

[Power Shell script for creating users](https://github.com/joshmadakor1/AD_PS)

##  Create a new virtual machine named "Client1" and install Windows 10 on it.

![Pasted image 20230402155056](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/e6cfe01b-9833-471d-a99e-ec0f64c2b61f)



##  Connect the client machine to the private network and join it to the domain.

![Pasted image 20230402155713](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/b61233e6-e10b-4012-ae72-31d762b3d083)


![Pasted image 20230402155807](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/5f749899-1574-4867-8f2d-d2d310b2e89e)


##  Log into the client machine with a domain account.

![Screenshot 2024-05-10 154749](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/e7a7c5fb-52be-4a3a-b861-552fc34ef8a1)


![Screenshot 2024-05-10 154836](https://github.com/Barry-Lenhart/Active-Directory-lab/assets/169422557/58ad1757-ba7b-40f8-aba6-fa45c93e1869)
