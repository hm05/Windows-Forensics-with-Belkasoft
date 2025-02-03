F1.1.  Where is the Master File Table (MFT) stored in NTFS?
```diff
- In a special file called @mft
+ In a special file called $MFT
- In the FAT table
- In the user folder
```
F1.2. What is the main purpose of Alternate Data Streams (ADSs) in NTFS?
``` diff
- To hide system files
+ To include multiple data streams apart from the main one
- To improve file system performance
- To track changes in files
```
F1.3. Which Windows artifact allows for quick access to the most recent files opened by apps via the 'Start' menu or 'Taskbar'?
```diff
- LNK files
+ Jump Lists
- Registry files
- Windows 10 Timeline
```
F1.4. Which of the following types of activities can be found in the Windows Timeline? 
Select all that apply
```diff
+ Opening documents
- Downloading files
+ Launching programs
+ Viewing videos
```
F1.5. You would like to check if a certain application was run on a machine under investigation. You cannot find any traces of execution in the UserAssist. What conclusion can you make? 
```diff
+ It does not mean that this application has not been run, as not all applications store data in UserAssist
- It means that the application has not been run during the last 30 days
- It means that the application has not been run since the last restart
- It means that the application has not been run on this machine
```
<!-- 
F1.6. You need to check if a suspect stored any illicit videos on his PC. You have checked the PC hard drives, but have found only 10 innocent video files. What can you do to make sure nothing is missed?
Select all that apply
```diff
+ Check if there are any additional video streams in the existing video files
- Analyse UserAssist and prefetch files
- Analyse RAM and page/hibernation files, if they are available
+ Carve the hard drives
```
-->
F2.1. Which website is mentioned in the ADS of the file image:\2\vol_344981504\Users\phorger\Downloads\powder.zip?
```diff
- https://powder.com
- https://powders.de
+ https://powdertoy.co.uk
- http://mypowder.com
```
F2.2. What link is provided in the email whose subject starts with “Police alert”?
```diff
- twitter.com
- stolenpassrecovery.com
+ virusexchange.home
- belkasoft.com
```
<!-- 
F2.3. For which sites is there evidence that they were used to find a gift for a girlfriend? 
```diff
- Forbes
+ Etsy
- Amazon
+ eBay
```
-->
F2.4. One of the data sources includes a banknote picture in PSD format. What value does the banknote have?
```diff
- 10 USD
- 20 USD
+ 50 USD
- 100 USD
```
<!-- 
F2.5: Which of the following VMware related logs can be found on the PC? .
Select all that apply.
```diff
+ vmware-vmusr-phorger.log
- vmware-vmsvc-phorger.log
+ vmware-vmusr-admin.log
- vmware-vmvss-SYSTEM.log
```
-->
<!-- 
F2.6: Which of the following website visits can be found only in the deleted (carved) browsing history?
```diff
- https://login.chinacloudapi.cn
- https://billthemegakill@icloud.com
+ https://albert.apple.com
+ https://www.bing.com
```
-->
F2.7. Traces of running which browsers can you find?
```diff
+ Chrome
+ Firefox
+ Microsoft Edge
- Opera
```
<!-- 
F2.8. Windows logged several attempts to login using explicit credentials. Which of the following target user names were used in these attempts?
Select all that apply.
```diff
+ phorger
- DWM-0
- DWM-1
+ DESKTOP-5B8Q7LT$
```
-->
F2.9. Check if an application with package hash HhfAoMceThjXij4yABiDYE8fi7j4tVlksBfxCSO2vY0= has been run on the user machine, and if yes, when it happened (UTC).
```diff
- It was run one time on July 11, 2018
- It was run several times on July 19 and July 20, 2018
+ It was run several times on July 20, 2018
- There is no information about this application launch
```
