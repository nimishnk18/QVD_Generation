# QVD_Generation

How to generate a QVD?

QVD stands for <b>QlikView Data </b> File. It is a native QlikView format which can be written to and read by QlikView.
<br>
It contains a single table of data and is optimized for fast loading.

A QVD file can be created by many different methods but we will be using the <b><i>Store</b></i> command in QlikView script.

<ol>The steps are as follows:
<li> If you have created a Data Source Object(DSO), double-click on that DSO ->Select Settings -> Enable the checkbox in front of External SAP HANA view
                                                      OR
<li> If you have created an Advanced Data Source Object (ADSO), login to Eclipse -> BW Modeling -> Double-click on your ADSO -> Enable the checkbox in front of External SAP HANA view

<li> Login to Eclipse -> SAP HANA Perspective -> Go to your DSO/ADSO -> Find the View which has been created for you (ADSO) or your own view (in case of DSO)
<li> Toggle to SQL Editor to view the SQL Query
<li> Copy the SQL Query
<li> Now logon to QlikView Desktop using Citrix Receiver. 

<li> Make sure you are working on QlikView Server. For that
  <ul>
 <li> Enter the server name as - qlikview.jbssa.com
 <li> Click Connect
 </ul>
 <li>Now open a new file and Click on Edit Script(CTRL+E)
 <li>Paste the SQL Query you copied
 <li> Edit the query to write the table name and Store the query into the specific location.
 <li> Use the INSERT statement in the main tab to Include SAP HANA -> Edit the statement to "MUST_INCLUDE(...)"
 <li>Save the file 
 <li> Hit the Reload Button
 <li> The QVD file is generated on the location specified.
 </ol>
 <li> Great Work ! Congrats 
 
 
 
 
 
 
