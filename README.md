# whatsyourcalling
Code for the demo site built. Team Bruh-grammers, IIT-M Ai challenge. Theme - Education.

Just don't look at the code already.

Read the proposal.pdf file.

The tech stack and algortihm have been tinkered a bit.

Read the writeup.pdf file.

Take a deep breath.

We'll setup the environment for the site to run.

1.Install node Js.

 https://nodejs.org/en/download/
 
2. Install npm

https://www.npmjs.com/get-npm
 
3. Install MySql 

This may take some time. When on Linux or Mac OS, you'll have a bit trouble concerning root access permissions.  
Google it ASAP. WE REPEAT, GOOGLE IT ! 

https://dev.mysql.com/doc/refman/8.0/en/installing.html

4. Install MySql Workbench.

5. Establish a connection between the workbench and MySql.

6. Install node js dependencies.
> npm install express body-parser ejs recommender http-server sentiment mysql nodemon

7. Open MySql workbench, create a new schema, name it db_connect
 
 *PLEASE TAKE EXTRA CARE IN DOING THIS STEP*
 
 Create a new table under this schema. 
 Name it 'new_table'
 Add these coloumns :
 

CREATE TABLE `db_connect`.`new_table` (
 `idnew_table` INT(11) NOT NULL,
 `title` VARCHAR(10000) NULL,
 `text` VARCHAR(40000) NULL,
 `aero` DECIMAL(10,9) NULL,
`chem` DECIMAL(10,9) NULL,
`civil` DECIMAL(10,9) NULL,
`cs` DECIMAL(10,9) NULL,
`ece` DECIMAL(10,9) NULL,
`eee` DECIMAL(10,9) NULL,
`mech` DECIMAL(10,9) NULL,
`user_1` DECIMAL(20,10)NULL,
`seen` INT(10)NULL,
 PRIMARY KEY (`idnew_table`));


 Create another table under this schema.
 Name it 'user_table'
 Add these coloumns :
 
iduser_table	int(11) PK
branch	varchar(45)
user_1	decimal(20,10)
 
 *NAME THE COLOUMNS AND THEIR DATATYPES CORRECTLY. CHANGING THIS A BIT, MAY MESS UP THE CODE* 
 
 
 8. Import results.csv file in new_table.

 9. Open index.js file. The code inside looks like spaghetti but does wonders.
 
 10. Fill in your DB connection information like username, password etc.,
 
 It's time for some action.
 
 Open up terminal / command prompt.
 
> node index.js

Visit http://localhost:3000/

WE HAVEN'T ADDED USER LOGIN FEAUTRE, YET. THE DEFAULT USER IS user_1. IF YOU WANT TO RESET HIS PREFERENCES, CLICK ON 'RESET' TAB ON FEED.

 
 Incase of a doubt, please feel free to reach out at jayasuriyars@gmail.com
 
 or through the contact number on the front page of the proposal.pdf file.
 
 