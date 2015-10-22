# SAS---Macro-Codes-
Storing a list of values from a data step into a macro 


proc sql; 
  select distinct country
  into :countries separated by ', '
  from orion.customer; 
quit; 

#separated by argument stores multiple values in a single macro variable
