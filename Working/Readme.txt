SAR Tool
-----------------------

The tool package consists of 4 files, 2 of them are critical:
-----------------------------------------------
1) the  .mbx file, which is the mapbasic execuable.
2) the  "SR_Seed.xls", which has the SR Form template

NOTE: please do not attempt to edit, separate or delete these 2 files.  They are required for the tool to run.


There are also 2 help files:
-------------------------------
1) the Sample Input File.xls which has an example of the required input xl file
2) this file....readme.txt




Before running the tool, please ensure the following:
------------------------------------------------------
xl settings
-------------
1) your xl security settings should enable macros in workbooks (at least they need to ask the user to enable macros)


input file
------------
1) the column headers must be exactly as shown in the sample input file, they do not have to be in that order though, you can also add your own columns
2) the column headers must be on the first row of the xl sheet (as shown in the sample input file
3) 4 columns (Lat/Lon/Search Ring Radius/Antenna Ht) must contain only numeric values
4) the lat and lon values should be always +ve numbers, the N/S and E/W denote the region (as per the export from 9155)

NOTE: the tool will reject the input file if it does not comply with these rules




Running the tool
---------------------
To run the tool simply run the .mbx file while you have mapinfo open with the maps you want to use as a backdrop in the search ring maps

The tool will create a toolbar (with 2 buttons), click the right button, then the left button and you are done


Left button
----------------
The left button imports your input data and creates the sites and search rings

The result will be 2 tables added to the mapper:
1) the "SAR Tool Sites" table, this table has the locations of the nominal sites
2) the "SAR Tool Rings" table, this table has the search ring objects

At this point you could replace the "SAR Tool Rings" table with your own search ring table (if you have custom search rings etc...)


Right Button
--------------
When you are ready to generate the search ring forms, press the right button

The tool will open xl and start communicating with xl to make the search ring forms 

NOTE: If an instance of xl is not already open on your PC, the tool will try to open xl.  With some office installations the tool can not open xl autonomously.
If this occurs, the tool will promt you to open an instance of xl.
-------------------------------------------------------------------

Tool written by Nathan Scott May09 - nathanpaulscott@yahoo.com