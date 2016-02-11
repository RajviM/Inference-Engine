# Inference-Engine
Modelled a knowledge representation system in First Order Logic. Backward Chaining was used as the inference procedure 

##Problem:  
Given a knowledge base and a number of queries.  The program determines if the queries can be inferred from the knowledge base or not.  
Solved this problem by making use of backward chaining.

##Input Format
1. Read file name from command line.
2. The first line of the input will be the number of queries (n).    Following n lines will be the queries, one per line.   Next line of the input will contain the number of clauses in the knowledge base (m).

#Rules
Each clause is in one of these two formats:  
1- p1 ∧ p2 ∧ ... ∧ pn => q  
2- facts: which are atomic sentences. Such as p or ~p 
All the p s and also q are either a literal such as HasPermission(Google,Contacts) or negative of a literal such as ~HasPermission(Google,Contacts).    Queries will not contain any variables.   
Variables are all single lowercase letters    All predicates (such as HasPermission) and constants (such as Google) are case-sensitive alphabetical strings that begin with uppercase letters.    
Each predicate has at least one argument. (There is no upper bound for the number of arguments). Same predicate will not appear with different number of arguments.   See the sample inputs for spacing patterns.   
All of the arguments of the facts are constants. i.e. you can assume that there will be no fact such as HasPermission(x,Contacts) ( which says that everyone has permission to see the contacts!) in the knowledge base.      
You can assume that the input format is exactly as it is described. There are no errors in the given input    

##Output
For each query, determine if that query can be inferred from the knowledge base or not, one query per line.   If true, print “TRUE” and if not, print “FALSE”. 

