Setup
===========
Create a workspace
-----------

    cd ~
    mkdir -p ros/src
    cd ros/src
    source /opt/ros/hydro/setup.bash
    catkin_init_workspace .
    cd ~/ros
    catkin_make
    source devel/setup.bash

optionally add `source ~/ros/setup.bash` to `.bashrc` in order to automatically have ros support in every terminal you open.

Clone au repositories
-----------
Enter the source directory

    cd ~/ros/src
    
Clone the dynamixel_motors package

    git clone https://github.com/au-crustcrawler/dynamixel_motor.git 
    
Clone the au_crustcrawler_base package

    git clone https://github.com/au-crustcrawler/au_crustcrawler_base.git
    
Clone the au_crustcrawler_moveit package

    git clone https://github.com/au-crustcrawler/au_crustcrawler_moveit.git
    
Clone the quickui package

    git clone https://github.com/au-crustcrawler/quickui.git
    
Enter the root workspace directory

    cd ~/ros
    catkin_make
    source devel/setup.bash
    
Whats next
---------
Look at the documentation for [au_crustcrawler_base](https://github.com/au-crustcrawler/au_crustcrawler_base/blob/master/readme.md) package
and [au_crustcrawler_moveit](https://github.com/au-crustcrawler/au_crustcrawler_moveit/blob/master/README.md) package

