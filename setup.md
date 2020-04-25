---
layout: page
title: Setup
---

WE ARE IN THE PROCESS OF UPDATING THESE INSTRUCTIONS. COME BACK SOON!

This lesson can be found in [https://osulp.github.io/matlab-novice-inflammation/](https://osulp.github.io/matlab-novice-inflammation/)

You will need access to MATLAB to follow this lesson. MATLAB is a MathWorks product that must be purchased. If you are an OSU faculty, staff or student, you have several options to install Matlab that we outline below. If you are not part of OSU MATLAB offers [30 day trials](https://www.mathworks.com/products/get-matlab.html). You can also follow this lesson using [GNU Octave][gnu-octave].

## If you use your own laptop and you want to install MATLAB in it. 

### MATLAB installation
You can get a license through OSU following the instructions in [https://is.oregonstate.edu/service/software/matlab](https://is.oregonstate.edu/service/software/matlab). 

### Data download for the class
You will also need to download some data, which we will analyze using MATLAB:

1. Make a new folder on your Desktop called *matlab-novice-inflammation*.
2. Download [matlab-novice-inflammation.zip]({{ page.root}}/data/matlab-novice-inflammation.zip) and move the file to this folder.
3. Extract the zip archive. This will place all the data in the `matlab-novice-inflammation` directory.
   Note that on Windows, double-clicking on the zip file simply previews the contents: to extract, right-click and select **Extract All**

## If you use your own laptop and you want to use Citrix

### MATLAB installation

* You will need to use Citrix. You have two options
	1. Install the Citrix receiver client in your computer following the instructions [here](https://it.engineering.oregonstate.edu/citrix). 
	2. Use Citrix in a browser by going to https://apps.oregonstate.edu and logging in with your e-mail and password. *This is a better option if you are doing this at the beginning of the class, it is faster*
		- If using **Firefox**: When prompted, activate the citrix plugin.
		- **IE** If you already have the citrix Workspace client, skip the install step and continue to the browser version of Citrix.
		- **Safari** When prompted, select "Trust" to unblock the Citrix Workspace plug-in.
		- **Chrome** elect "Use light version" when prompted to "Detect Receiver/Workspace"
	
* Find MATLAB on the Apps tab. Double click on the MATLAB icon. After a minute or so MATLAB should open. 

### Data download
When you use MATLAB via Citrix MATLAB will only see the folders in your ONID Drive space. Unfortunately there is no way to have MATLAB access the files in your local computer. To access your ONID storage space from your personal computer do the following:

#### Via Citrix

* Open the Chrome app on Citrix Apps here: http://apps.oregonstate.edu 
* Navigate to this lesson and download [matlab-novice-inflammation.zip]({{ page.root}}/data/matlab-novice-inflammation.zip). The file will appear at the bottom of the page. Click on the arrow and choose "Show in folder". (the file will be downloaded in Network/onid-fs.onid.oregonstate.edu/youronidusername/Profile/Downloads/)
* On the explorer folder right click on the file matlab-novice-inflammation. You will get a Windows Security message. Click OK. Chose Copy.
* Through the navigation panel on the left navigate to This PC -> ONID Home (Z:). Create a folder called *matlab-novice-inflammation*. Inside the folder right click and choose Paste. 

#### Windows On-Campus (or from home connected via VCN)

1. From the windows search bar type "\\onid-fs.onid.oregonstate.edu"
2. Type in your ONID user name "onid\Username" and password
3. You will see two folders: public_html and a folder with your onid user name. Save files in your user folder. This directory will show up as the Z drive from applications running from apps.oregonstate.edu

Once you can see the ONID Drive from your computer, download the data:

1. Make a new folder on your ONID Drive called *matlab-novice-inflammation*.
2. Download [matlab-novice-inflammation.zip]({{ page.root}}/data/matlab-novice-inflammation.zip) and move the file to this folder.
3. Extract the zip archive by right-clicking and selecting Extract all. Note that on Windows, double-clicking on the zip file simply previews the contents. This will place all the data in the `matlab-novice-inflammation` directory.

Alternative instructions in [this OSU article](https://oregonstate.teamdynamix.com/TDClient/KB/ArticleDet?ID=45710)

#### Mac On-Campus 

1. Open finder. On the top menu chose Go, and then Connect to server.
2. Add smb://onid-fs.onid.oregonstate.edu to the server to connect, and press Connect.
3. Enter your ONID information. Name "onid\username" and password
4. Choose the right volume to connect to. It should be the one named as your ONID username. 
5. The drive should appear in your finder window as onid-fs.onid.oregonstate.edu

Once you can see the ONID Drive from your computer, download the data:

1. Make a new folder on your ONID Drive called *matlab-novice-inflammation*.
2. Download [matlab-novice-inflammation.zip]({{ page.root}}/data/matlab-novice-inflammation.zip) and move the file to this folder.
3. Extract the zip archive. This will place all the data in the `matlab-novice-inflammation` directory.

Alternative instructions in [this OSU article](https://oregonstate.teamdynamix.com/TDClient/KB/ArticleDet?ID=45703)

#### Off campus

To connect via VPN follow instruction in https://oregonstate.teamdynamix.com/TDClient/1935/Portal/KB/ArticleDet?ID=76790 and follow instructions above. 

For instructions on accessing ONID Drive from a Windows or a Mac off campus check the articles in [this OSU page](https://oregonstate.teamdynamix.com/TDClient/KB/ArticleDet?ID=45671). 



You will need to install MATLAB or  to do this lesson. If you are an OSU faculty, staff or student, you have several options to install Matlab:

1. You can install MATLAB with an OSU license 
2. You can access MATLAB without having to install it in your own computer using [Citrix](https://it.engineering.oregonstate.edu/citrix).
3. You can use one of the computers in the Autzen classroom during the workshop. These computers do not have a local Matlab installation, we will use [Citrix](https://it.engineering.oregonstate.edu/citrix)

**If you use Citrix** 
You will need to install the Citrix receiver client following the instructions [here](https://it.engineering.oregonstate.edu/citrix), identify yourself with your ONID, and find MATLAB on the Apps tab. Double click on the MATLAB icon and you should be all set. 

It can be a little confusing to find where to save your documents when using Citrix. Review [the documentation](https://it.engineering.oregonstate.edu/citrix) under "How to turn on/off access to local hard drive and USB" and "How to access local drives while using an app in Citrix" to figure that out. If you are using a classroom computer we recommend saving your files in the Z drive, so your documents will stay in your ONID account. If you are using your own computer you will want to save them locally (in the "C" drive). Instructions for connecting to your ONID home directory from your computer [here](http://oregonstate.edu/helpdocs/onid-osu-network-id/connecting-onid/your-home-directory). 

# Download data for the workshop

You will also need to download some data, which we will analyze using MATLAB:

1. Make a new folder on your Desktop called *matlab-novice-inflammation*.
2. Download [matlab-novice-inflammation.zip]({{ page.root}}/data/matlab-novice-inflammation.zip) and move the file to this folder.
3. Extract the zip archive. This will place all the data in the `matlab-novice-inflammation` directory.
   Note that on Windows, double-clicking on the zip file simply previews the contents: to extract, right-click and select **Extract All**
4. You can access this folder from the Unix shell with:

	~~~
	cd Desktop/matlab-novice-inflammation/data
	~~~
	{: .bash}

[gnu-octave]: https://www.gnu.org/software/octave/
