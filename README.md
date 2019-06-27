# QVD_Generation

How to generate a QVD?

QVD stands for <b>QlikView Data </b> File. It is a native QlikView format which can be written to and read by QlikView.
<br>
It contains a single table of data and is optimized for fast loading.

A QVD file can be created by many different methods but we will be using the <b><i>Store</b></i> command in QlikView script.

<ol>The steps are as follows:
<li> If you have created a Data Source Object(DSO), double-click on that DSO ->Select Settings -> Enable the checkbox in front of External SAP HANA view
  <br>
  <img width="924" alt="ADSO_SAP Hana View" src="https://user-images.githubusercontent.com/30903014/60287543-61ebb400-98cf-11e9-9337-9e5e7489d160.PNG">
                                             <br> 
                                                      OR
                                               <br>
<li> If you have created an Advanced Data Source Object (ADSO), login to Eclipse -> BW Modeling -> Double-click on your ADSO -> Enable the checkbox in front of External SAP HANA view
<br>
  <img width="924" alt="ADSO_SAP Hana View" src="https://user-images.githubusercontent.com/30903014/60287865-361cfe00-98d0-11e9-941b-36f71650c07e.PNG">
<br>
<li> Login to Eclipse -> SAP HANA Perspective -> Go to your DSO/ADSO -> Find the View which has been created for you (ADSO) or your own view (in case of DSO)
  <br>
 
<li> Toggle to SQL Editor to view the SQL Query
  <br> <br>
  <img width="952" alt="Sql_editor" src="https://user-images.githubusercontent.com/30903014/60299076-134b1380-98e9-11e9-833f-0526f0c8db65.PNG">
<br>
<li> Copy the SQL Query
  <br><br>
  <img width="823" alt="copy sql" src="https://user-images.githubusercontent.com/30903014/60298811-90c25400-98e8-11e9-81b2-7ae09f56cf61.PNG">
  <br>
<li> Now logon to QlikView Desktop using Citrix Receiver. 
<br><br>
  <img width="612" alt="Citrix Sc" src="https://user-images.githubusercontent.com/30903014/60299834-e0098400-98ea-11e9-8e83-9299a3d5195a.PNG">
  
<br>
<li> Make sure you are working on QlikView Server. For that
  <ul>
 <li> Enter the server name as - qlikview.jbssa.com
 <li> Click Connect
 </ul>
 <li>Now open a new file and Click on Edit Script(CTRL+E)
 
 <li> Go to your Main Tab -> Use the INSERT statement -> File Name - \\USTXCRQLKF1I -> Qlik -> QlikViewStorage -> Include -> Extraction -> SAP HANA BHD/BHQ/BHP 
  <li>
   Edit the statement inserted as "MUST_INCLUDE("......").
   
   <br><br>
   <img width="653" alt="include sc" src="https://user-images.githubusercontent.com/30903014/60299284-99fff080-98e9-11e9-8fb7-3e7bc398af43.PNG">
   <br>
   <br><br>
   <img width="479" alt="include sc2" src="https://user-images.githubusercontent.com/30903014/60299475-0549c280-98ea-11e9-9251-6b11bf288c67.PNG">
   <br>
   
   <br><br>
   <img width="629" alt="must_include" src="https://user-images.githubusercontent.com/30903014/60299496-15fa3880-98ea-11e9-8b78-e2dfdc93b22e.PNG">
   <br>
   <li>Paste the SQL Query you copied in a new tab
 <li> Edit the query to write the table name and Store the query into the specific location.
<br> <br>
<img width="463" alt="table_name" src="https://user-images.githubusercontent.com/30903014/60299806-d2ec9500-98ea-11e9-8717-9f0504a8b139.PNG">
<br>
  <br> <br>
  <img width="438" alt="store_function" src="https://user-images.githubusercontent.com/30903014/60299802-cff1a480-98ea-11e9-9cd4-3fbc7583c8ff.PNG">
  <br>
<li>Save the file 
 <li> Hit the Reload Button
   <br><br>
   <img width="779" alt="Hit_Reload" src="https://user-images.githubusercontent.com/30903014/60299854-eb5caf80-98ea-11e9-9215-0a1d64e2ef64.PNG">

   <br>
 <li> The QVD file is generated at the location specified.
 </ol>
 
 Great Work! You have successfully created a QVD.
 
 
 
 
 
 
