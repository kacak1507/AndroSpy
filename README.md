# AndroSpy - Xamarin-C# Android RAT  
<img src="https://user-images.githubusercontent.com/45147475/89324496-096d1580-d690-11ea-86d2-1b8b1d484d35.png" width="25%"></img>   

An Android RAT that written in completely C# by me.

<img src="https://user-images.githubusercontent.com/45147475/110235549-ae5f1200-7f41-11eb-8fbc-40beb79ecff5.PNG" width="55%"></img>  

Yes, It is supporting dns connection like no-ip or duckdns or dynu etc. and it has been tested with ngrok and portmap.io; it is working with both but you can't hear live mic because of UDP port.  

Your Visual Studio must have Xamarin Developing Kit, otherwise you can't build client.  

If you have Xamarin Developing Kit;  

Building Tutorial: https://www.youtube.com/watch?v=MbZJDwBrvDE  

# Compilation
## Step 1:
[!] COMPILE THE CLIENT PROJECT IN VISUAL STUDIO ONCE, THEN YOU MAKE IN BOTTOM STEPS, OTHERWIESE YOU SEE ERROR IN BUILDER. 
--> (THIS STEP IS REQUIRED BECAUSE OF NUGET PACKETS.) If you see Nuget Packages errors in Visual Stuido, download this .zip and extract to path of Client project https://www.mediafire.com/file/eeuakup61xhz5iv/packages.zip/file then close Visual Studio and re-open the Client project (Task2.sln), then clean project and re-build the Client project.  

## Step 2:
[!] Then you must put path of each .exe in Settings window of AndroSpy and copy the all files of Client project to "ProjectFolder" path in SV project (\SV\bin\Debug\resources\ProjectFolder)  

[!] Important: Select MSBuild.exe from your Visual Studio installed path, not from .NET Framework;  

      {Installed Drive of Visual Studio}\Microsoft Visual Studio\{VERSION}\{EDITION}\MSBuild\Current\Bin\MSBuild.exe;  
      
             
<img src="https://user-images.githubusercontent.com/45147475/107190577-01ee4680-69fc-11eb-9da3-2088a35e4696.PNG" width="45%"></img>  

<img src="https://user-images.githubusercontent.com/45147475/107374011-30514c00-6af8-11eb-9452-f056c7f20dbb.PNG" width="45%"></img> <img src="https://user-images.githubusercontent.com/45147475/107373882-0e57c980-6af8-11eb-9fb9-bf6336f5252d.PNG" width="45%"></img> <img src="https://user-images.githubusercontent.com/45147475/107373887-0ef06000-6af8-11eb-8bc6-8a50287296ad.PNG" width="45%"></img>  

<img src="https://user-images.githubusercontent.com/45147475/107262779-05142180-6a52-11eb-932e-492b5deef531.PNG" width="45%"></img>  

After making the settings in the above pictures, you can now create clients.  

+ Microphone issue after recent Android 10 update:  
+ https://forum.xda-developers.com/t/microphone-issue-after-recent-android-10-update.4085727/page-2

## Builder
<img src="https://i.imgur.com/v4Av2FM.png">

-------------------------------------------------------------------------------------------------------------------------

Don't worry, there is no complicated ``Socket`` programming; all thing is simple to understand.  

-You must also UDP port open; select item in comboBox on NAT page of Modem: TCP and UDP (both) , otherwise you can't hear live microphone.    

For Keylogger your victim must toggle on Accessibility button of your trojan in Settings of Device  

<img src="https://user-images.githubusercontent.com/45147475/101618575-3e64ec80-3a23-11eb-8462-8d36606878d3.jpg" width="25%"></img>

Minumum Android Version: 4.1    

Tested on some systems:  
Android 4.4.2 - OK  
Android 5.1.1 - OK  
Android 7.1.2 - OK  
Android 6.0.1 - OK  
Android 9.0   - OK  
Android 10    - OK  

AndroSpy Project aims to most powerful-stable-useful open source Android RAT.  

After installing backdoor on device, it will show popup box for screen share, please accept this box and check "Don't show again".  

Working with all network types: 2G, 3G, 4G, 4.5G, WI-FI.....; not only working in the local network, but in the WAN.  

Frequently check for update on github repo of AndroSpy for the best user experience.  

For Huawei and other EMUI devices, read this article: https://dontkillmyapp.com/huawei I added the code suggestion for developers to our Client; wakelock tag: "LocationManagerService"  

(The Images below are not up to date pictures.)

<img src="https://user-images.githubusercontent.com/45147475/107142142-e6bd0180-693d-11eb-90e3-7c9bc6209616.PNG" width="45%"></img>  

<img src="https://user-images.githubusercontent.com/45147475/123464904-1707f280-d5f6-11eb-95e0-a6a87c164a92.png" width="60%"></img>  

<img src="https://user-images.githubusercontent.com/45147475/110211525-f4679780-7ea7-11eb-93fc-8a325769cf0b.PNG" width="45%"></img>  <img src="https://user-images.githubusercontent.com/45147475/110211526-f598c480-7ea7-11eb-936b-68f14aa4fa27.PNG" width="45%"></img>  <img src="https://user-images.githubusercontent.com/45147475/110211528-f6315b00-7ea7-11eb-8098-4f24e70b7cf8.PNG" width="45%"></img>    <img src="https://user-images.githubusercontent.com/45147475/110211530-f893b500-7ea7-11eb-8709-d4b5a7267632.PNG" width="45%"></img>  

<img src="https://user-images.githubusercontent.com/45147475/110211527-f6315b00-7ea7-11eb-8f48-fde920293420.png" width="23%"></img> 

# Update 24.07.2021  

+ Re-connect issue permanently fixed (thanks to ping-pong method.) (reconnecting if timeout is 15 seconds).  
+ Some changes, edits etc.  

# Update 25.06.2021  

+ Re-connect issue fixed.  
+ Added Shell Terminal.  
+ Added toolTip ping status (0m 0s 30ms) (move mouse on to image of victim)
+ Live Camera was improvement.  
+ Socket comminication was improvement.  
+ Added RAM and Internal Storage informations. (with toolTip)  
+ Some visual improvements (Text Fonts, words etc.)  
+ Added charging status image and wifi signal strength image. (with toolTip)  
+ and others...  

# Update 20.05.2021  

+ Added CPU-Wakelock option to Builder. (high connection performance)  
+ Builder options are now saved automatically.  
+ Visual changes (all windows now can be maximized)
+ Memory leak optimisations.
+ Code optimisations.
+ Some minor changes & fixs & improvements

# Update 21.04.2021  

+ Fixed a minor bug in File Manager
+ Fixed Installed Apps icon above android 9.0  
+ Some minor changes & fixs & improvements

# Update 06.03.2021 - Ertuğrul Bey Edition  

+ I just want to say this; use and see.

# Update 21.02.2021  

+ Switching to Service based application.  
+ Few improvements.  

# Update 07.02.2021 - Dracula Edition  

+ The GUI has been completely redesigned.  
+ The Builder error has been fixed (errors caused because of misused "/" marks)  
+ Some stabilisation improving.  
+ And others that I have forgot to write here.... :)  

# Update 30.01.2021 - Fusion Edition  

+ You can multiple operation handle; multiple files upload and download, while watch live cam or screen watch, download or upload files multiple.  
+ Builder error fixed. Now there no will be error.  
+ Performance increased.  
+ while Doze Mode (sleep mode) your victim can connect by hand Alarm Manager to server and communicate wtih you.  
+ If server has no internet, victim can re-connect to server while internet avaible on Server.  
+ Snapshot from camera is currently disabled by me. [I'm too lazy for re-coding this for new Socket instance :)].  
+ Added settings for emui devices(huawei, oppo, honor etc....) for background working.  
+ and some bug fixing, performance stabilisations etc......

# Update 2021 Jan. 24  

+ Socket communication has been completely re-coded; quality camera view, fast and light communication. Communicate entirely with byte[] arrays; It got rid of Base64, Fast and light communication.
+ The graphical user interface has been renewed.
+ File download and sending codes, photo capture codes were re-coded by creating a buffer zone.
+ "Night mode" has been added to the live camera form and live screen form.
+ Close, Reconnect and Remove options have been added for the client.
and other improvements-fixes ..  

# Update December 2020 on Version 3  

+CPU Wakelock is now choose of user in Builder.  
+Added "Password" properties for connection security between you and your client.  
+WakeLock power usage optimized; our client uses as little battery as possible.  
+Added "Detailed Infos" tab in the Status of Phone Window, you can see; detailed IMEI, SIM Infos and more..  
+High CPU usage problem fixed that has caused when device didn't have Internet.  
+Focus Mode on Live Camera is now choose of User.  
+Added Live Screen (MediaProjection API has been available since API Level 21, for more: https://developer.android.com/reference/android/media/projection/MediaProjection  
+File Manager has been improvement.  
+Fully English version.  
+Now it is supporting 5 digits Port.  
+Fixed English Flag issue.  
+If device does not have any camera, you will see warning message.  
+Added victim name and ip adress as title of control windows. Ex: Keylogger - Victim@192.168.2.78:7675  
and other changes, fixing, improvents. :)

# Version 3  
+Added live Camera stream (with resolution,zoom,flash,quality controls and scene,focus,white balance mode)  
+Fixed loss data transfer  
+Some excess codes have been removed  
+Performance has been increased

# [+] Update on version V2  
+Added logs.  
+Added preview of clicked image into the filemaneger.  
+Added choose sizes of both front and back camera.  
+Some other fixes and changes.

# [+]Version Update 2 (first update as version)  
+Switching to ``System.Net.Sockets.NetworkStream`` from directly ``System.Net.Sockets.Socket`` Communitation. This change was more stable and fast. And Project has cleaner code.  
+Added Wifi,Bluetooth,Mobil Data etc. into  the Phone Infos form.  
+Added screen brightness option into the settings panel.  
+Some important updates-changes.

# [+]Update 1.3 (First stable Update)  
+Added "Add Shortcut to home screen" option into the Fun Manager.  
+Added Name of Phone Number into the Window that is showed when Incall or Outgoing Call starts in any Victim.  
+a Correction in SMS Manager.

# [+]Update 1.2 ( semi-stable Update :) )  
+Connection between Client and Server has been improvement.  
+Added 'Name' column into the Sms and Call Log manager.  
+Some visual changes.  
+Added dropped Pin URL into the Location Manager  
+Fixed terminate problem that caused by Ram Cleaner.  
+Fixed problem that caused when our trojan hides self from launcher.  
+Our trojan can hide it self from launcher.

# [+]Update 1.1  
+Major improvements  
+Added Flash/Torch option to Camera Manager and percentage status with progressbar.  
+Reconstructed Upload/Download file and added percentage status with progressbar.  
+Added Download Manager (you can download any file that you want into the victim's phone but you must put filename into textBox)  
+Added some features into Call Manager (Send sms to selected phone number directly, call selected number...)
+Added source into Microphone Manager (Mic, Call, Default)  
+Some visual improvements.
And more that I have forgot to write :)

# [+]Update 1.0  
+Critical improvements (in both Server and Client)  
+Re-made File Manager (more sightly, stable and useful)

# [+]Update 0.1.2  
+some improvements (in both Server and Client)  
+Notify when Call (incoming or outgoing) in any client starts.  
+Camera was improvement.
