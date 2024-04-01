# Lab-PostGIS  
<figure width=100%>
  <IMG SRC="https://www.colorado.edu/cs/profiles/express/themes/cuspirit/logo.png" WIDTH=50 ALIGN="right">
</figure>
    
## CSCI 3287 
<hr>
  
 **This assignment takes longer. Please start early** <br>
 **Please submit the pdf printout via gradescope.
Make sure it include the results and full SQL command in the printout to avoid missing points**
<hr>

#### You're going to use the PostGIS database with GIS extensions to analyze <br> four data sets involving bars, windmills (turbines), roads and state outlines.
The individual datasets are provides as either ZIP files containing SHP/DBF files, GeoJSON or JSON. The notebook contains code to load the datasets in the files as GeoPandas notebooks. You will need to transfer that data to the PostGIS database.

#### You will be creating tables in your MySQL server database.

The https://coding.csel.io system has all the required extensions and libraries needed to conduct the homework. You should split your work into two phases:

* In the first, you should work on getting your data into PostGIS. I've provided assistance for you to check if you have the proper number of rows of data in your database. This process will take ~10 minutes depending on your network connection.
* In the second, you should start authoring the queries #1-#8. If you need to go away for a while and then restart, your data will be in the database, but you'll need to re-connect to the database. You won't need to reload the data.
<hr>

When you're done with the assignment, *push your changes to your remote repository and print a PDF of your results. The queries increase in difficulty and the last query will probably require you to use a **WITH** query, also known as a **Common Table Expression (CTE)**.<br>
( see [https://dev.mysql.com/doc/refman/8.0/en/with.html](https://dev.mysql.com/doc/refman/8.0/en/with.html) )
