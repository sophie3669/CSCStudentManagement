Queries that can be made on the database
// this selects all the field content in the CSCStudent Table
1. SELECT QUERY
SELECT * FROM CSCStudent

// this selects specific year one results with regards to the specified regno and then Renames the table 
2. SELECT CSC101Result, CSC102Result, CSC103Result,CSC111Result, CSC121Result FROM Year1CSCSubjectScores As MyYearOneResult WHERE RegNo= "2009514692"

//this updates the 300 level result for a particular regno.
3. UPDATE Year3CSCSubjectScores
SET CSC301Result=50,CSC341Result=70,CSC351Result= 100, CSC300= 66 
WHERE StudentRegNo= "2009514696";

//this deletes a particular table with respect to the reg number specified.
4.  DELETE FROM Year2CSCSubjectScore
WHERE RegNo="2009514692";

//this inserts a new column into a particular table
5. INSERT INTO Year1CSCSubjectScores(CSC101Result, CSC102Result, CSC103Result, CSC111Result)


VALUES (30,66,10,23);
