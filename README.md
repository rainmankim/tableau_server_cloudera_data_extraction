<img align="left" src="https://user-images.githubusercontent.com/62319355/105784986-d6f40380-5fb4-11eb-95e9-2261360d0120.jpg" width="220" height="80" alt="Tableau Server">
<img align="right" src="https://user-images.githubusercontent.com/62319355/105791113-6eab1f00-5fc0-11eb-938c-58db40f72c20.png" width="150" height="80" alt="Cloudera logo">
:smile: :grinning: :sleepy: :relieved: :confused: :open_mouth: :astonished: :thumbsup:


# tableau_server_cloudera_data_extraction


```
Creator: Ray Kim Dong Hyun
Contact: rainmankim@gmail.com

* For easier understanding, I am going to call Tableau Server "Ray's Tableau Server".

This repository will show you the following in the following order:
- (1) Connect Tableau Desktop with Cloudera Hadoop Server
- (2) Enter custom SQL to extract necessary data
- (3) Publish data source onto "Ray's Tableau Server" with emedded authetification as LIVE data source
- (4) From "Ray's Tabealu Server", change the data from LIVE to EXTRACT  (takes a while)
- (5) Open a new Tableau Desktop instance and connect to the publisehd data source
```


### Step 1.  Let's open up Tableau Desktop and connect to Cloudera Hadoop with your credentials
<img align="center" src="https://user-images.githubusercontent.com/62319355/105792845-10337000-5fc3-11eb-9fd8-43d35e496f13.png" alt="tableau_cloudera_connection image">


## Before starting, I recommend that you prepare two things
### (1) Ensure your scripting is enabled on your SAP.
<img align="center" src="https://github.com/rainmankim/SAP_automation_python/blob/master/images/scripting_pic.png" alt="SAP image">

#### You might need to request your IT department to allow this.
### (2) Download Stefan Schnell's SAP Script Recorder.
#### SAP has a built-in recorder. But if you use that you will need to change the syntax to be used in Python.
#### Using Stefan's Recorder generates Python-friendly syntax along with many other powerful features.
<img align="center" src="https://github.com/rainmankim/SAP_automation_python/blob/master/images/tracker.gif" alt="Tracker image">
https://tracker.stschnell.de/



## Next, open any Python IDE/code editor. 
## I recommend Jupyter Notebook so that you can slice data in-action.
### Below is an example of recorded scripts which are modified to suit my needs (*for loops + various conditions)
<img align="left" src="https://github.com/rainmankim/SAP_automation_python/blob/master/images/jupyter_snapshot.PNG"  alt="Jupyter image">


## I have two main functions in my file — def sap_automate()  and def enter_data()
### sap_automate(df) is the main function that will establish connection/session and automate log-in
### enter_data(session,df) is a nested function that will execute actions within SAP
<img align="left" src="https://github.com/rainmankim/SAP_automation_python/blob/master/images/jupyter_snapshot_main.PNG"  alt="Jupyter image">


## Dealing with Excel
### If you are writing to an existing excel, Pandas library would be not be enough
### Use Excel modules such as xlwings or xlsxwriter

## Credits
```
- Secular saints of Tableau Community
```


