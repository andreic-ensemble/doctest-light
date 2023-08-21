---
title: Installation Guide
description: Installation Guide
---

# Installation

Apache ZooKeeper is a centralized service for maintaining configuration information across a RadiantOne cluster. Although RadiantOne comes bundled with ZooKeeper to simplify installation in Dev/QA environments, it is discouraged to use this architecture in production. Shutting down a redundant RadiantOne node (e.g. for upgrading) also shuts down ZooKeeper on this server. Because a ZooKeeper ensemble must have a quorum of more than half its servers running at any given time, this can be a problem for cluster integrity and stability. The solution is to deploy ZooKeeper in a separate, external ensemble. Other advantages of deploying an external ZooKeeper ensemble are outlined in the RadiantOne External ZooKeeper Install guide.

For details on installing RadiantOne in a Dev/QA environment, where ZooKeeper is installed and configured on the RadiantOne node, follow the steps outlined in this installation guide.

For details on installing RadiantOne in a production environment, start with the steps in the [RadiantOne External Zookeeper Installation Guide](/documentation/external-zookeeper-install-guide/01-introduction) to setup the external ZooKeeper ensemble. Then, refer to the steps in this guide to install RadiantOne.

## Installer Files

The installer files are available on the Radiant Logic support site. Contact support@radiantlogic.com for access information.

RadiantOne can be installed via a web-based GUI wizard, or through a silent (non-GUI) installer. The installer files are described below in the table below.



| Installer File | Description
|------------|------------|
| radiantone_<version>_full_linux_64.tar.gz  for Linux platforms that includes RadiantOne documentation. Untar the file to the location you want the product installed and then use setup.sh to install | This is used for a [silent install](#silent-mode-installs) or [GUI-based install](#gui-based-install) for Linux platforms that includes RadiantOne documentation. Untar the file to the location you want the product installed and then use setup.sh to install the RadiantOne platform with a GUI, or use install-sample.properties with Instance Manager to install in a silent mode. <br> radiantone_<version>_full_linux_64.tar.gz.512 is the corresponding checksum (SHA512 hashing algorithm) associated with the installer file. 
| radiantone_<version>_full_windows_64.zip  for Linux platforms that includes RadiantOne documentation. Untar the file to the location you want the product installed and then use setup.sh to install | This is used for a [silent install](#silent-mode-installs) or [GUI-based install](#gui-based-install) for Windows platforms that includes RadiantOne documentation. Extract the contents of the compressed file to the location you want the product installed, and then use setup.bat to install the RadiantOne platform with a GUI, or use install-sample.properties with Instance Manager to install in a silent mode. <br> radiantone_<version>_full_windows_64.zip.sha512 is the corresponding checksum (SHA512 hashing algorithm) associated with the installer file.

