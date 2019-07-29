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

#### Windows On-Campus 
Find instructions in [this OSU article](https://oregonstate.teamdynamix.com/TDClient/KB/ArticleDet?ID=45710)

#### Mac On-Campus 
Find instructions in [this OSU article](https://oregonstate.teamdynamix.com/TDClient/KB/ArticleDet?ID=45703)

For instructions on accessing ONID Drive from a Windows or a Mac off campus check the articles in [this OSU page](https://oregonstate.teamdynamix.com/TDClient/KB/ArticleDet?ID=45671). 

Once you can see the ONID Drive from your computer, download the data:

1. Make a new folder on your ONID Drive called *matlab-novice-inflammation*.
2. Download [matlab-novice-inflammation.zip]({{ page.root}}/data/matlab-novice-inflammation.zip) and move the file to this folder.
3. Extract the zip archive. This will place all the data in the `matlab-novice-inflammation` directory.
   Note that on Windows, double-clicking on the zip file simply previews the contents: to extract, right-click and select **Extract All**

## If you use a classroom computer using the Mac option

## If you use a classroom computer using the Windows option

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
