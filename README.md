# apt-cyg
## A Cygwin Command-line Package Manager

The original apt-cyg, which is [transcode-open/apt-cyg](https://github.com/transcode-open/apt-cyg), is taken down by DMCA for unknown reason.  
This script seems to be abandoned for a long time.  
I forked the code and decided to maintain the code by myself.  

- - -

A command-line software installer for Cygwin.  
Original version is available in http://code.google.com/p/apt-cyg/.

This tool can provide you the similar experience as apt-get in OSes of Debian family.  
For example, you can install unzip using this command.

    $ apt-cyg install unzip

and all the dependencies will be automatically installed as well.
You can execute this for further help.

    $ apt-cyg --help


## Installation
First you need to install git, wget, tar, gawk, xz and bzip2 using the Cygwin's official installer.
Then you can execute these commands in your Cygwin console:

    $ git clone https://github.com/fsgmhoward/apt-cyg 
    $ cp apt-cyg/apt-cyg /bin/ 
    $ rm -rf apt-cyg # if the local repository is not necessary 

## Usage
This version can be used similiarly to the original apt-cyg. I will tried to post a manual later. You can use `--help` for the usage of apt-cyg.  
The script will automatically detect your system's architecture and you do not need to set it manually.  
However, if you want to specify mirror site using `-m`, you are required to put x86 (for 32 bit machine) or x86_64 (for 64 bit machine) at the end of the mirror URL.

    $ apt-cyg update -m ftp://mirror.mcs.anl.gov/pub/cygwin/x86_64/

Generally it is more convinent to set the mirror address in the script by editing this line so that you do not need to use `-m` every time.

    mirror=ftp://mirror.mcs.anl.gov/pub/cygwin


## License
Copyright (C) 2005-9, Stephen Jungels  
Copyright (C) 2013, rcmdnk  
Copyright (C) 2016, Howard Liu  

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

[http://www.fsf.org/licensing/licenses/gpl.html](http://www.fsf.org/licensing/licenses/gpl.html)