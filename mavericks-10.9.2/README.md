Creating a wine wrapper for Autostakkert2
=================



## 1: Download Autostakkert2 and unzip
http://www.autostakkert.com/


## 2: Download and install wineskin winery
http://wineskin.urgesoftware.com/

Run wineskin and install the latest engine and wrapper.

![Screenshot](screenshots/winery.png "Winery")


## 3: Create a new wrapper for AutoStakkert2.

![Screenshot](screenshots/wrapper.png "Winery")

When it asks to download Mono and Geko click cancel as they are not needed.

When finished, click view wrapper in finder

![Screenshot](screenshots/wrapper-finished.png "Winery")

Now open the package contents (right click 'show package contents')

![Screenshot](screenshots/pkg-contents.png "Winery")

Run the wineskin application inside the contents and click install software

![Screenshot](screenshots/install-sw.png "Winery")

Click copy a folder inside

![Screenshot](screenshots/copy-folder.png "Winery")

Now select the downloaded and unzipped autostakkert2 folder.

![Screenshot](screenshots/copy-as2.png "Winery")

It will prompt for the exe to use. Click OK to return to the winery application.

![Screenshot](screenshots/exe.png "Winery")

Click advanced and then screen options

![Screenshot](screenshots/advanced.png "Winery")![Screenshot](screenshots/screen-opts.png "Winery")

Select 'Use Mac Driver insdead of X11'

You can perform a 'Run Test' from the advanced options to make sure it runs.

Close winery

## 4: Run Autostakkert

The wrapper will get created in the Applications folder in your home directory. Drag and drop from here into Applciations or just run from here.

If the application does not start then open a terminal and delete the launchctl for the application using this command

```no-highlight
launchctl remove $(launchctl list | grep wineskin | awk '{ print $3 }')
```


![Screenshot](screenshots/as2-running.png "AS2")
