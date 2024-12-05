# Setting Up Server 2016

## Software Used:
VirtualBox, Server 2016 Evaluation

## Obtaining Server 2016 ISO file

> Note that you first need to download virtualbox from the internet. You just look up virtualbox download on a browser, and it should be the first or second option. Look for an option to download that suits your computer specifications, and click download. Open the installation file and follow the prompts. From there, you should be set.

Open your web browser, and paste the following link: https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2016

It should take you to a screen that looks like this:

<img src="https://i.ibb.co/c3LrT04/1-Microsoft-Eval-Center.png">

From here, you could go on and download other versions of Windows Server. If you hover on the top where it says Windows Server, it will show a list of Server software that is available for download. But, for now, we will use Server 2016. So, click on "Download the ISO".

This will take you to a screen that says "Evaluate Server 2016" or something similar. On the side, a form will appear, just like this:

<img src="https://i.ibb.co/5jkRTcd/2-Register-for-your-free-trial-today.png">

Fill in the relevant information. If you don't have a company (most don't), make up a company name and a role. It's just for information. The contact information you provide will help you obtain free training from microsoft if that is what you want. At the end of the form, you will find a blue button that says "download now". Click that button.

This will take you to a page where you are able to choose what version of Windows Server you want to try. In our case, we want to try the 64-bit ISO. So click where it says 64-bit edition.

<img src="https://i.ibb.co/wJvgT7v/4-Download-64-bit.png">

> Make sure you locate where the file is downloaded. You could do this by going to File explorer, or by dragging the downloaded file to your desktop. The important thing is that you know where the file is, since you will need that information later.

## Creating a Virtual Machine (VM) on VirtualBox

Open up VirtualBox, and follow the steps on the following image:

> For step 3, just make sure those options are placed.

<img src="https://i.ibb.co/j8mh2LX/5-CVE-New-Virtual-Machine.png">

Then, the following screen will pop-up.

<img src="https://i.ibb.co/cJ5yQP4/6-Choosing-hardware.png">

This is showing you options of the "hardware" your virtual machine may have. You can leave the defaults, or customize depending on the hardware on your actual computer. In my case, I am using a laptop, so the defaults are fine. After this, we can hit next. 

This screen pops up:

<img src="https://i.ibb.co/p4cnqNK/7-Virtual-Hard-Disk.png">

Once again, the defaults are fine. We click next, and the following screen pops up.

<img src="https://i.ibb.co/RcQRVTG/8-Summary.png">

Here, you'll see a summary of the options you just chose. Verify they are correct, and click Finish. Now, your virtual machine is created. 


## Downloading Server 2016 on VM
By this point, you should have a screen that looks something like this:

<img src="https://i.ibb.co/vxZbVgJ/9-Start.png">

Click on Start. This will start up your VM. However, since there is no operating system (OS) installed, the following message will pop-up, asking you to insert bootable media. 

<img src="https://i.ibb.co/swN9YPD/10-Decide-boot-order.png">

To choose a bootable media, (in our case, the ISO file we downloaded previously) click on the drop-down arrow beside DVD. This will open File Explorer, where we are able to look for the ISO file we downloaded. Once we select the file, and click open on File Explorer, the name of the File will be placed beside DVD. Verify that it is the correct file, and click Mount and Retry Boot. It might take a while to load, but then a Windows setup screen should apppear. 

<img src="https://i.ibb.co/LgfpPNn/13-Windows-setup.png">

A good practice is to verify the information before we click next. In my case, the information is correct, so we click next. 

A screen saying "Install Now" will pop-up. Click Install Now. 

Various options for download will appear. Choose the Windows Server 2016 Standard Evaluation (Desktop Experience). This will allow us to use Server 2016 like a computer. On the bottom, it explains that this version uses a GUI or Graphical User Interface. It's basically telling you it's going to look like windows, rather than just being a command-line. Once we select this option, we click next.  

Accept the license agreement, and click next. 

A screen asking you what type of installation you want will appear. The two options are an upgrade, and a custom install. Since we are installing Windows Server from scratch, we will choose a custom install. 

<img src="https://i.ibb.co/0ZtTFHM/17-Custom-install.png">

Now, it will prompt you to partition the drive for the install. We don't need to do anything for this to happen, so we just need to click Next. 

<img src="https://i.ibb.co/5rN1ngC/18-Partition.png">

After that, Server 2016 should start downloading, and a screen will pop up that shows you that this is happening. Just let it do its thing. It should reboot after that. 

## Setting Up Admin Account
You should be greeted with a screen prompting you to create a password for your admin account.

<img src="https://i.ibb.co/rb8nhqK/20-Setting-up-password.png">

Once you create a password, click Finish. You will see the following screen:

<img src="https://i.ibb.co/X39649t/21-control-alt-delete.png">

For VirtualBox, to press ctrl + alt + delete, you have to go to the input tab, then to keyboard, and then to a button that says "insert ctrl+alt+delete". After that, you are able to log in, and...

CONGRATS! You've set up Server 2016!
