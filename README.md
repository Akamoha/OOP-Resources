This document contains instructions for setting up various software applications you would need in the OOP course.

---------------------------------
### 1. Java SE SDK
1. Download Java SE SDK from http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html; You have to accept the Oracle license agreement.
2. The file "jdk-8u51-linux-x64.tar.gz" is downloaded to your downloads location, typically ~/Downloads/ directory. (If you are using a 32-bit OS, choose the 32-bit version of JDK)
3. Right click on the zip file and select extract here option. A new sub-directory named 'jdk1.8.0_51' shall be created in ~/Downloads/ directory.
4. Open command terminal and login as root using the command `sudo su`. You need to provide the administrator's password to login as superuser.
5. Move the 'jdk1.8.0_51' directory to a system location.

    ```
    mkdir /usr/local/java  
    mv jdk1.8.0_51 /usr/local/java/
    ```
6. Create system-wide links to common Java commands

    ```update-alternatives --install "/usr/bin/java" "java" "/usr/local/java/jdk1.8.0_51/bin/java" 1
    update-alternatives --set java /usr/local/java/jdk1.8.0_51/bin/java
    update-alternatives --install "/usr/bin/javac" "javac" "/usr/local/java/jdk1.8.0_51/bin/javac" 1
    update-alternatives --set javac /usr/local/java/jdk1.8.0_51/bin/javac
    update-alternatives --install "/usr/bin/javaws" "javaws" "/usr/local/java/jdk1.8.0_51/bin/javaws" 1
    update-alternatives --set javaws /usr/local/java/jdk1.8.0_51/bin/javaws
    ```
7. Give up administrator's privileges.

     `exit`
8. Open your profile settings file.

     ```
     cd ~
     gedit .profile
     ```
9. At the end of the '.profile' file create a few blank lines and copy-paste the following lines
     ```
     JAVA_HOME=/usr/local/java/jdk1.8.0_51
     JRE_HOME=$JAVA_HOME/jre
     PATH=$PATH:$JAVA_HOME/bin:$JRE_HOME/bin
     export JAVA_HOME
     export JRE_HOME
     export PATH
     ```
10. Save and close the '.profile' file.
11. In the terminal, type `. .profile` to reload your bash shell profile.
12. Check the java version with `java -version` command. You should see version printed on terminal.
	```
	Java(TM) SE Runtime Environment (build 1.8.0_51-b16)
	Java HotSpot(TM) 64-Bit Server VM (build 25.51-b03, mixed mode)
	```
13. Now you are ready to develop Java programs using Java SE 7 development kit.
14. There are a whole bunch of useful development tools in the '/usr/local/java/jdk1.8.0_51/bin' folder. You can make these tools available to yourself by logging in as administrator and completing the instructions given in step#6 for each of the required tools.

For more detailed and graphical installation instructions, visit http://www.wikihow.com/Install-Oracle-Java-on-Ubuntu-Linux

### 2. Greenfoot
1. Visit http://www.greenfoot.org/download and click on the link for Ubuntu.
2. When this is done, navigate to your Downloads directory; you will find a file named "greenfoot-242.deb".
3. Double click this file to start the installation. It takes a while as it has to download ~60MB of data.
4. Once it's done, the installation is complete and you can start using Greenfoot by accessing it through the search bar.

### 3. Visual Paradigm Community Edition
1. Visit [http://www.visual-paradigm.com/download/community.jsp?platform=linux](http://www.visual-paradigm.com/download/community.jsp?platform=linux)
2. Select the InstallFree tar file under More Options and download the .tar.gz file.
3. Extract the downloaded .tar.gz file into a folder named "Visual Paradigm" in the Desktop (using Ubuntu's Archive Manager).
4. This creates a subdirectory named "Visual Paradigm 12.0" where 12.0 is the version number. That's it. To start Visual Paradigm, execute /Visual Paradigm 12.0/Visual Paradigm (click on the file in the folder)
5. To get activation code, enter a valid email id and get the input activation code in email. Use that to activate Visual Paradigm. ![image](https://cloud.githubusercontent.com/assets/5674080/9276299/949221d2-42c0-11e5-869c-72eb4d7d1c9f.png)

### 4. StarUML
1. Visit http://staruml.io/download and click on the 64-bit Ubuntu download.
2. After the download is done, click on the .deb file which is downloaded.
3. It will get installed through the Ubuntu Software Center.
4. You can then access it through the search bar.

### 5. Git
1. Download and install Git from http://git-scm.com/download/linux. Find the command pertaining to your ditribution. Linux Mint users follow the same instructions as Ubuntu.  
    NOTE: You may need superuser privileges to install Git. Prefix `sudo` before the actual command. For eg, for Ubuntu users -  
    `sudo apt-get install git`.
2. Follow instructions at https://help.github.com/articles/set-up-git/#platform-linux to configure Git.

### 6. Maven
1. Go to http://maven.apache.org/download.cgi to download the latest version of Maven. Download either the *Binary tar.gz archive* or *Binary zip archive* from under the *Files* subheading.
2. Extract the archive using *Archive Manager* or any one of the following commands -  
    `unzip apache-maven-3.3.3-bin.zip` or `tar xzvf apache-maven-3.3.3-bin.tar.gz` (for Maven 3.3.3)
3. Now open up the file `.profile` in your home directory for editing -  
    `sudo vi ~/.profile`
4. Append the following line to add the *bin* directory of your Maven folder to the *PATH* environment variable  
    `PATH=$PATH:/path/to/apache-maven-3.3.3/bin`
5. Logout of your user session and login again to reflect the changes. Enter `mvn --version` to see if Maven has been installed correctly. Your output should look similar to
	```
    Apache Maven 3.3.3 (7994120775791599e205a5524ec3e0dfe41d4a06; 2015-04-22T17:27:37+05:30)  
    Maven home: /path/to/apache-maven-3.3.3  
    Java version: 1.8.0_51, vendor: Oracle Corporation  
    Java home: /usr/lib/jvm/java-8-oracle/jre  
    Default locale: en_IN, platform encoding: UTF-8  
    OS name: "linux", version: "3.13.0-37-generic", arch: "amd64", family: "unix"
	```

### 7. NodeJS
Open up the terminal and execute the following command:

`sudo apt-get install nodejs`

### 8. NodeJS Package Manager (npm)
Open up the terminal and execute the following command:

`sudo apt-get install npm`

### 9. BlueJ
1. Visit http://www.bluej.org/
2. Scroll down to the section for Ubuntu/Debian Linux. Click on the link named "BlueJ Installer" and it will download a 6.5MB .deb file.
3. Once that's done, go to your Downloads directory and double click the .deb file to open it up in the Ubuntu Software Center.
4. Click the Install button to the right to begin installation.
5. It's quite a lightweight IDE so the installation shouldn't take long. Once it's done, you can then access it through the search bar.


### 10. App Inventor
The App Inventor website provides detailed instructions on how to download and install the software.

1. Visit http://appinventor.mit.edu/explore/content/linux.html
2. Follow the set of 5 instructions given under the heading "For systems that can install Debian packages"

### 11. Mozilla Firefox Add-ons
Mozilla Firefox should already be installed on your systems. Follow these steps to install the required add-ons for it:

1. Firebug: Visit https://addons.mozilla.org/en-US/firefox/addon/firebug/ and click the "Add to Firefox" button.
2. Web Developer: Visit https://addons.mozilla.org/en-us/firefox/addon/web-developer/ and click the "Add to Firefox" button.
3. RESTClient: Visit https://addons.mozilla.org/en-US/firefox/addon/restclient/ and click the "Add to Firefox" button.

### 12. Eclipse IDE
1. Visit https://eclipse.org/downloads/ and download the 64 bit or 32 bit version of "Eclipse IDE for Java EE Developers", depending on your system. This is a 268MB file so it'd be better if you downloaded it from DC instead.
2. Extract the Eclipse installation tarball into your home directory:

	```
	cd
	tar -xzvf <path/to/tar-file>
	```

3. Increase the memory for the Eclipse installation by modifying the ~/eclipse/eclipse.ini file: Change the -Xmx setting (line 20) to be at least 1G (i.e. make it -Xmx1024m). Also change the -XX:MaxPermSize (line 18) to at most 512m.
4. Run Eclipse:

	`~/eclipse/eclipse`
