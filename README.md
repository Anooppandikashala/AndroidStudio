# Android Studio Installations(Ubuntu and Windows):

Before going to install the android studio and all others please check the following..

1. In BIOS Secure booting is ```off``` or ```disable```
2. Enable hardware acceleration. For more info Goto [Link](https://2nwiki.2n.cz/pages/viewpage.action?pageId=75202968)
3. In Ubuntu Check the kvm status For more info Goto [Link](https://www.alibabacloud.com/blog/how-to-install-and-configure-kvm-on-ubuntu-18-04_595501)

## 1. Ubuntu:

1. Install java (Oracle java): Goto [Link](https://drive.google.com/open?id=17XZY3wBfin_wJ6RMRj8V3h58PqWp-LRK)

2. Download  ```jdk-8u231-linux-x64.tar.gz ``` file
3. Download  ```install-java-master.zip``` file and extract it.


### 1.1 Java Installation

Extract ```install-java-master.zip```

The script ```install-java.sh``` needs to be run as root.

You need to provide the JDK distribution file (`tar.gz`) and the Java Installation Directory. The default value for Java installation directory is "/usr/lib/jvm"

```console
$ sudo ./install-java.sh -h

Usage: 
install-java.sh -f <java_dist> [-p <java_dir>]

-f: The jdk tar.gz file.
-p: Java installation directory. Default: /usr/lib/jvm.
-h: Display this help and exit.

```
Example: Installing Oracle JDK 8

```console
$ sudo ./install-java.sh -f ~/pathto-jdk-downloaded/jdk-8u231-linux-x64.tar.gz 
Installing: jdk-8u231-linux-x64.tar.gz
Extracting /home/path-to-jdk/jdk-12.0.1_linux-x64_bin.tar.gz to /usr/lib/jvm
JDK is extracted to /usr/lib/jvm/jdk-8.0.1
Run update-alternatives commands? [y/N] 
Do you want to set JAVA_HOME environment variable in /home/isuru/.bashrc? [y/N]
```

### Automate Java Installation

You can automate the Java installation script by using the `yes` command.

### 1.2 Android Studio Installation

1. Goto : [Link](https://developer.android.com/studio?gclid=EAIaIQobChMIrOebs9CF5wIVzQorCh1uhAL6EAAYASAAEgLm2_D_BwE)

2. Download Latest Installer from the website.
3. Extract the zip file into home directory
4. Open the extracted folder and navigate to bin folder
5. Right click open the terminal from the folder 
6. in terminal type

```console
$ ./studio.sh
```

7. follow the installer.

### Or Install from the software center :

Please follow the link [Link](https://vitux.com/how-to-install-android-studio-ide-on-ubuntu/)


### 2.3 Testing and setting-up Android Studio

1. Open Android Studio

2. Create A Desktop entry

![Opening window](https://github.com/Anooppandikashala/AndroidStudio/blob/master/desktop_entry.png)

2. Setting up Android SDK

![Android SDK](https://github.com/Anooppandikashala/AndroidStudio/blob/master/sdk_manager_0.png)

From this select SDK Tools and install ticked(checked) packages and hit apply
![Android SDK](https://github.com/Anooppandikashala/AndroidStudio/blob/master/sdk_manager_1.png)

3. Setting up JDK-8 Replace default jvm

![Android SDK](https://github.com/Anooppandikashala/AndroidStudio/blob/master/project_structure.png)
![Android SDK](https://github.com/Anooppandikashala/AndroidStudio/blob/master/default-jvm.png)
change the default to installed java-8 (Example-in ubuntu)```Please note Windows path may change```
it is the path to the java installed folder.
![Android SDK](https://github.com/Anooppandikashala/AndroidStudio/blob/master/installed_java_8.png)




### 1.3 Genymotion installation (```Light weight Android Emulator- Only for personal usage```)

1. Goto [Link](https://www.genymotion.com/fun-zone/)
2. Or Download it from [Link](https://drive.google.com/open?id=17XZY3wBfin_wJ6RMRj8V3h58PqWp-LRK) (```genymotion-3.0.4-linux_x64.bin```)
3. Download Virtual box from 
    [Link](https://drive.google.com/open?id=17XZY3wBfin_wJ6RMRj8V3h58PqWp-LRK) (```virtualbox-6.1_6.1.0-135406_Ubuntu_bionic_amd64.deb```)

    1. Download the file and Right click the ```virtualbox-6.1_6.1.0-135406_Ubuntu_bionic_amd64.deb``` and open with software center.
    2. install the virtual box.
4. After installing Virtual box we can start installing Genymotion
5. Goto downloaded folder of ```genymotion-3.0.4-linux_x64.bin``` and  right cick and open in terminal from the folder.
6. In terminal type

```console
$ cp genymotion-3.0.4-linux_x64.bin  ~/.
$ cd 
$ chmod a+x genymotion-3.0.4-linux_x64.bin
$ ./genymotion-3.0.4-linux_x64.bin
```

7. Follow the installer.

## Now you Successfully installed Java, Android Studio and Genymotion In Ubuntu.


## 2. Windows:

### 2.1 Java Installation:

1. Goto [Link](https://drive.google.com/open?id=17XZY3wBfin_wJ6RMRj8V3h58PqWp-LRK) and download ```jdk-8u241-windows-x64.exe```
2. Double click and run the installer and follow the installer.

3. For more info goto [Link](https://www.shaileshjha.com/step-by-step-how-to-download-and-install-java-se-jdk-8-on-windows-10/)

### 2.2 Android Studio Installation:

1. Goto [Link](https://developer.android.com/studio/) and download the installer for Windows (Recommended installer)

2. After downloading the installer run the .exe file and follow the installer.
 ```For detailed info Goto : ``` [Link](https://www.onlinetutorialspoint.com/android/how-to-install-android-studio-on-windows-10.html)
 


### 2.3 Genymotion installation (```Light weight Android Emulator- Only for personal usage```)
 
1. Goto [Link](https://www.genymotion.com/fun-zone/)  and  download ```installer for Windows (With Virtualbox )```
![With Virtualbox](https://github.com/Anooppandikashala/AndroidStudio/blob/master/image004.jpg)
2. To download the installer, you have to create a free account on Genymotion.
3. After downloading, run the installer.
4. Follow the installer.
5. For more info Goto [Link](https://acadgild.com/blog/install-genymotion-windows)
6. Please note download the ```installer with Virtualbox```

### OR
7. Download the exe file from [Link](https://drive.google.com/open?id=17XZY3wBfin_wJ6RMRj8V3h58PqWp-LRK)
8. From the folder find out ```genymotion-3.0.4-vbox.exe``` and download it.
9. Run the installer and Follow the installer.

## ******* You Successfully installed all the components *******



