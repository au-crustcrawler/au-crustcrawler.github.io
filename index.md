Setup
===========
Create a workspace
-----------

    cd ~
    mkdir -p catkin_ws/src
    cd catkin_ws/src
    source /opt/ros/hydro/setup.bash
    catkin_init_workspace .
    cd ~/catkin_ws
    catkin_make
    source devel/setup.bash

optionally add `source ~/catkin_ws/devel/setup.bash` to `.bashrc` in order to automatically have ros support in every terminal you open.

Clone au repositories
-----------
Enter the source directory

    cd ~/catkin_ws/src
    
Clone the dynamixel_motors package

    git clone https://github.com/au-crustcrawler/dynamixel_motor.git 
    
Clone the au_crustcrawler_base package

    git clone https://github.com/au-crustcrawler/au_crustcrawler_base.git
    
Clone the au_crustcrawler_moveit package

    git clone https://github.com/au-crustcrawler/au_crustcrawler_moveit.git
    
Clone the quickui package

    git clone https://github.com/au-crustcrawler/quickui.git
    
Enter the root workspace directory

    cd ~/catkin_ws
    catkin_make
    source devel/setup.bash

Configuring Eclipse
---------
This guide is based on C/C++ Eclipse Indigo version.
Install the pydev plugin from the following update-site.

    http://pydev.org/updates

It is important to install version 2.8.2 this is done by unchecking the *Show only the latest versions of available software*. 


Then get catkin (cmake) to generate an eclipse project for your workspace.
A single project is being generated with all the packages in one project.

    catkin_make --force-cmake -G"Eclipse CDT4 - Unix Makefiles"

Then in eclipse select *import -> existing project* and then select *~/ros/build* as the root folder and select Project@Build project. Do not select copy projects into workspace.

source link [ROS IDE](http://wiki.ros.org/IDEs).

Remeber to use the catkin steps and not the old deprecated rosbuild steps. 


Whats next
---------
Look at the documentation for [au_crustcrawler_base](https://github.com/au-crustcrawler/au_crustcrawler_base/blob/master/readme.md) package
and [au_crustcrawler_moveit](https://github.com/au-crustcrawler/au_crustcrawler_moveit/blob/master/README.md) package

