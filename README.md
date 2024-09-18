# Workspaces Images
This repository contains several example of desktop and application Workspaces images.
Administrators may leverage these images directly or use them as a starting point for their own custom images.
Each of these images is based off one of the [**Workspaces Core Images**](https://github.com/kasmtech/workspaces-core-images?utm_campaign=Github&utm_source=github) which contain the necessary wiring to work within the Kasm Workspaces platform.


For more information about building custom images please review the  [**How To Guide**](https://kasmweb.com/docs/latest/how_to/building_images.html?utm_campaign=Github&utm_source=github)

The Kasm team publishes applications and desktop images for use inside the platform. More information, including source can be found in the [**Default Images List**](https://kasmweb.com/docs/latest/guide/custom_images.html?utm_campaign=Github&utm_source=github)

# Kasm-Ubuntu22.04-Image-Template
Template workspace for Kasm servers, includes base applications such as Google Chrome, as well as Canvas for students and other apps default on school provided computers.


## For making and changing versions use the following commands:

```bash
docker login

sudo docker build -t nighthawkcoders/pusd-student-ubuntu:1.14.0-csa . 
docker push nighthawkcoders/pusd-student-ubuntu:1.14.0-csa 
```
(replace 1.14.0-csa with the version you want to make, also the . is important so make sure you use it)
- important note: make sure to match the versions both in the commands as well as in the kasm_registry repo also for me it kept saying permission denied when pushing so try not using sudo if it says that after logging in.