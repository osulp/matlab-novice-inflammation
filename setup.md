---
layout: page
title: Setup
---

This lesson can be found in [https://osulp.github.io/matlab-novice-inflammation/](https://osulp.github.io/matlab-novice-inflammation/)

You will need to install MATLAB or [GNU Octave][gnu-octave] to do this lesson. If you are an OSU faculty, staff or student, you have several options to install Matlab:

1. You can install MATLAB with an OSU license following the instructions in [https://is.oregonstate.edu/service/software/matlab](https://is.oregonstate.edu/service/software/matlab). 
2. You can access MATLAB without having to install it in your own computer using [Citrix](https://it.engineering.oregonstate.edu/citrix).
3. You can use one of the computers in the Autzen classroom during the workshop. These computers do not have a local Matlab installation, we will use [Citrix](https://it.engineering.oregonstate.edu/citrix)

**If you use Citrix** 
You will need to install the Citrix receiver client following the instructions [here](https://it.engineering.oregonstate.edu/citrix), identify yourself with your ONID, and find MATLAB on the Apps tab. Double click on the MATLAB icon and you should be all set. 

It can be a little confusing to find where to save your documents when using Citrix. Review [the documentation](https://it.engineering.oregonstate.edu/citrix) under "How to turn on/off access to local hard drive and USB" and "How to access local drives while using an app in Citrix" to figure that out. If you are using a classroom computer we recommend saving your files in the Z drive, so your documents will stay in your ONID account. If you are using your own computer you will want to save them locally (in the "C" drive). Instructions for connecting to your ONID home directory from your computer [here](http://oregonstate.edu/helpdocs/onid-osu-network-id/connecting-onid/your-home-directory). 

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
