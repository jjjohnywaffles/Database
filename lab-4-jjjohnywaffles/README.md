## CSCI 3287 - Lab ER Diagram to Databasse
<figure width=100%>
  <IMG SRC="https://www.colorado.edu/cs/profiles/express/themes/cuspirit/logo.png" WIDTH=50 ALIGN="right">
</figure>
	
In this homework, you're going to take your completed E/R diagram and the database tables you created in your CSPB mySQL database and populate the tables with data. <br>
___You will need to create triggers and constraints on the data for fields.___   
You will need to write triggers for handling the deletion of records in one table that are depend upon in other tables.   
___We will access your database to validate the tables.___

You will create and clear your tables using SQL commands in your JupyterLab notebook.  <br>
___You must use the JupyterLab notebook to populate your database with table entries.___

You will need to use Git to ___commit___ your updated notebook (Lab_4.ipynb) to your local repository. <br> You will need to ___push___ your commits to the remote repository in Git Classroom.   <br>
___We will access your remote repository to validate your SQL statements in your notebook.___

<hr>
 
### There are three items to complete for this assignment:
	
1. Create Tables, Triggers, and Table Data in your CSPB MySQL database via your JupyterHub Notebook. 
2. Push your Lab_4.ipynb changes to the remote repository under Git Classroom.
3. Submit the information listed below into this Moodle assignment.

     * Your name
     * CU ID: (4 letters - 4 digits)
     * GitHub ID:
     * \# of hours it took to complete the lab

#### Here are the rules for populating your database tables:

* Must use a series of INSERT statements in your JupyterLab notebook.  Hint: you should probably clear the tables at start of the notebook.

* Create at least 3 teams.
* Each team must have at least 3 players.  (Remember that players can only belong to one team)
* Create at least 3 games.   Each game must have:
  * at least one pass play
  * at least one run play
  * at least 3 players involed in plays
  * at least one pass play of more than 25 yards
  * at least one running play of more than 10 yards
  * at least one play for each team
 <br><br>
 
* Every player must be assigned to a team.  You will need to order the INSERT operations to handle the constraints 

#### Use the JupyterLab notebook to show the state of the tables

* Show the state of your databases using __```select *```__ for __Team__, __Player__, __Plays__ and __Game__.

* Provide a SQL query to show the roster for each team, listing the team name and player names.

* Provide a SQL query to show the plays for each game, 
  * all plays are listed in one table, ordered by the  __Team__ id, __Game__ id
  * show __Team__ name, __Game__ id, 
  * If the play is a "pass" indicate that "X passed to Y", where X and Y are player names 
  * If the play is a run indicate "X ran", where X is a player name 
  * To handle the play type, [you may want to use a CASE statement](http://www.mysqltutorial.org/mysql-case-function/)
  * Indicate the yardage in another column
<br><br>

* Using  a ```__try...except__ block```,  attempt to INSERT an existing player from the first team into the second team. This should raise an exception and fail.

* Delete one of your __Teams__. This should cascade a series of changes:
  * deleting the __Player__ records for that team
  * deleting the __Plays__ for that player 
  * deleting any __Game__ for that __Team__
<br><br>

* Show the database state after the deletes, using a __```select *```__ for __Team__, __Player__, __Plays__ and __Game__. 

