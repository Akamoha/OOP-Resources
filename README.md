This document contains instructions for setting up various software applications you would need in the OOP course.

---------------------------------
### 1. Java SE SDK
1. Download Java SE SDK from http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html; You have to accept the Oracle license agreement.
2. The file "jdk-8u51-linux-x64.tar.gz" is downloaded to your downloads location, typically ~/Downloads/ directory. (If you are using a 32-bit OS, choose the 32-bit version of JDK)
3. Right click on the zip file and select extract here option. A new sub-directory named 'jdk1.8.0_51' shall be created in ~/Downloads/ directory.
4. Open command terminal and login as root using the command `sudo su`. You need to provide the administrator's password to login as superuser.
5. Move the 'jdk1.8.0_51' directory to a system location.   
    `mkdir /usr/local/java`  
    `mv jdk1.8.0_51 /usr/local/java/`
6. Create system-wide links to common Java commands   
    `update-alternatives --install "/usr/bin/java" "java" "/usr/local/java/jdk1.8.0_51/bin/java" 1`   
    `update-alternatives --set java /usr/local/java/jdk1.8.0_51/bin/java`   
    `update-alternatives --install "/usr/bin/javac" "javac" "/usr/local/java/jdk1.8.0_51/bin/javac" 1`      
    `update-alternatives --set javac /usr/local/java/jdk1.8.0_51/bin/javac`   
    `update-alternatives --install "/usr/bin/javaws" "javaws" "/usr/local/java/jdk1.8.0_51/bin/javaws" 1`   
    `update-alternatives --set javaws /usr/local/java/jdk1.8.0_51/bin/javaws`   
7. Give up administrator's privileges.   
     `exit`
8. Open your profile settings file.   
     `cd ~`   
      `gedit .profile`
9. At the end of the '.profile' file create a few blank lines and copy-paste the following lines   
     `JAVA_HOME=/usr/local/java/jdk1.8.0_51`   
      `JRE_HOME=$JAVA_HOME/jre`   
      `PATH=$PATH:$JAVA_HOME/bin:$JRE_HOME/bin`   
      `export JAVA_HOME`   
      `export JRE_HOME`   
      `export PATH`   
10. Save and close the '.profile' file.
11. In the terminal, type `. .profile` to reload your bash shell profile.
12. Check the java version with `java -version` command. You should see version printed on terminal.   
     `Java(TM) SE Runtime Environment (build 1.8.0_51-b16)`   
     `Java HotSpot(TM) 64-Bit Server VM (build 25.51-b03, mixed mode)`
13. Now you are ready to develop Java programs using Java SE 7 development kit.
14. There are a whole bunch of useful development tools in the '/usr/local/java/jdk1.8.0_51/bin' folder. You can make these tools available to yourself by logging in as administrator and completing the instructions given in step#6 for each of the required tools. 

For more detailed and graphical installation instructions, visit http://www.wikihow.com/Install-Oracle-Java-on-Ubuntu-Linux

### 2. Greenfoot
1. Visit http://www.greenfoot.org/download and click on the link for Ubuntu.
2. When this is done, navigate to your Downloads directory; you will find a file named "greenfoot-242.deb".
3. Double click this file to start the installation. It takes a while as it has to download ~60MB of data.
4. Once it's done, the installation is complete and you can start using Greenfoot.

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
