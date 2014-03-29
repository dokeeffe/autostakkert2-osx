autostakkert2-osx
=================

Wrapper for Autostakkert2 to run in OSX


1: Download Autostakkert2
http://www.autostakkert.com/


2: Download and install wineskin winery
http://wineskin.urgesoftware.com/
Run wineskin and install the latest engine and wrapper.

3: Create a new wrapper called AutoStakkert2
When it asks to download Mono and Geko click cancel as they are not needed.


4: Add autostakkert to the wrapper and configure


5: Run Autostakkert






launchctl remove $(launchctl list | grep wineskin | awk '{ print $3 }')
