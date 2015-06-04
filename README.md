Max Lichtenstein's pi-camera

Intro:

This is a set of utilities for managing timelapse and web cameras using the "motion" program on a raspberry pi.

Getting started with git:
clone the github into the top level, so:

cd /
sudo mkdir pi-camera
sudo chmod 777 pi-camera
git clone https://github.com/mlichtenstein/pi-camera

and wait for the magic!

Now that you've got the repo,
setting up motion:

sudo apt-get install motion

duh.  Then, you want motion to point to your git repo.  I did this a hacky way:  add this to your .bashrc:

alias motion="motion -c /pi-camera/motion.conf -p /pi-camera/motion.pid"


