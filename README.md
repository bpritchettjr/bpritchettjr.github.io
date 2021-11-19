**Note: Create Specific Documents for each project.**

This Document includes the steps to run the scripts in a virtual ubuntu environment on a windows host operating system via VirtualBox.


#### Step 1: Install Virtualbox

Virtual box is a tool which allows you to run different operating systems virtually on your host operating system. This is referred to as a virtual machine.
	
In order to install Virtualbox, follow this link:

https://www.virtualbox.org/wiki/Downloads

Under “VirtualBox 6.1.28 platform packages” select the windows host download link.

Open VirtualBox

#### Step 2: Download Ubuntu ISO file

For the purposes of this document I will be utilizing ubuntu 20.04, although  18.04 is recommended. 

Follow this link:

https://ubuntu.com/#download

Under the Download button select 20.04 LTS

#### Step 3: Set Up Ubuntu virtual machine in virtualbox

Open virtualbox

Click the “New” button

Provide the name of your new machine (I recommend the name Ubuntu 20.04)

Set Machine folder location(your choice)

Ensure the Type and version fields are correct (Type: Linux ; Version: Ubuntu(64-bit))

Select Next

Select memory size (Anywhere inside the green area of the scale)

Select Next

Select “Create a virtual hard disk now”
Select Create

Select VDI(Virtual Disk Image)

Select Next

Select Dynamically Allocated (Allows the OS to expand disk size if required)

Select Next

Choose File Location

Choose virtual Hard disk size(I recommend around 100Gb)

Click Create

#### Step 4: Configure Settings for Ubuntu Virtual Machine

Select your machine

Select Settings

Under General, click advanced settings. Select Bidirectional for both shared clipboard and drag and drop fields. This will allow you to share files between host machine and ubuntu machine.

Under System, click processor. Choose the number of CPUs you wish to use. (if no preference leave as default)

Under storage Click empty. Under attributes, by optical drive click Disk dropdown and select choose a disk file. Provide location for ISO file downloaded in step 2.

Select OK.

#### Step 5: Open your virtual machine

Select your machine and press start.

Select preferred language and click install ubuntu

Select Keyboard Layout and Language, Click Continue

Under “What apps would you like to start with?” Select normal installation

Under “Other Options” select download updates while installing ubuntu and Install third party software for graphics and Wi-Fi hardware and additional media formats

Click continue

Under Installation Type, Select Erase Disk and install ubuntu

Click Install Now

Click continue

Select your Location

Enter your preferred Name, Username and Password

Click Continue.

Wait for installation to complete.

Click Restart Now.

Log in to the user you created

Follow Setup Instructions provided by the OS.  

#### Step 6: (Optional) Install Virtual Box Guest Additions

This software will allow your virtualbox virtual machine to properly maximize on your screen

Open Terminal

Give command: sudo apt install build-essential dkms linux-headers-$(uname -r)

Provide your password

Enter y, press enter

Close terminal

Select devices on virtualbox window

Select Insert Guest additions CD Image

Select Run

Provide your password, click authenticate

Restart ubuntu operating system

