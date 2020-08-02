# Y1-Sem2-Lab4
its late and i doubt anyonr will ever see this :)

1. Summer 2018: Rewrite the code in the chooseLargest function below to use zip (), lambda and map(). You can assume the output of 
map is cast to a list.       
def chooseLargest (a, b):   
  result = []     
  for i in range (len(a)):    
    result.append(max(a[i], b[i]))   
   return result 
 
l1 = [1, 2, 3, 4, 5]  l2 = [2, 2, 9, 0, 9]  chooseLargest (l1, l2) 

2. Summer 2018: Assume you have a file called lotteryNumbers.txt. This contains the winning lottery draws 
(6 numbers for each draw) for the last year, with each draw on a separate line and the numbers separated by a single space. 
Example:  23 30 5 8 18 14 11 10 3 17 18 20 ... 
Write the code to read this file into a list called lotteryDraws. 
Each draw within this list should be a list of integers.  Call the function read_draw() and return the list 

3. Summer 2018: Consider a courier company that has 10 drivers, numbered 0 to 9, that records the number of deliveries by 
each driver, over a 5 day week with days numbered 0 to 4, in a table having 10 rows and 5 columns. Thus, for example, the 
entry in row 7 and column 3 gives the number of the deliveries by driver number 8 on day number 2. 
Assuming that a table, courierData, has already been filled with data, write two separate Python functions 
which take this table as an input parameter and return: 
Return the total number of days on which at least 1000 deliveries were made. Call the function del_1000(courierData) 
Return the number of the driver who made the most deliveries in the week (assume there can only be one).  
Call the function most_del(courierData) 

4. Autumn 2018: Rewrite the code below to use lambda and map(). You can assume the output of map is cast to a list. 
You should still zip the two lists.     
def append_list(): 
  list1 = [1,2,3] 
  list2 = [10,20,30] 
  totals = [] 
  for tup in zip(list1, list2):  
    totals.append (tup[0] + tup[1]) 
    return (totals) 
   
 5. Autumn 2018: Data Consulting Agency (DCA) needs you to develop software to match their clients. The list of 
 clients is in a text file with one line per client. The following is an example of six clients although you should 
 assume the client list to be larger.
 
John Smith, M, 27, F, 24, 29, movies, tennis, walking, computers 
Alison Jones, F, 25, M, 26, 32, walking, golf, movies, reading 
Brian Adams, M, 30, F, 23, 28, golf, cricket 
Chris Jones, M, 27, F, 30, 40, golf, reading 
Paul Fulton, M, 23, M, 21, 25, football, reading 
Peter Jackson, M, 25, M, 20, 30, golf, walking, movies 

The file specifies information about the client. For example, John Smith is male, 27 years old and wishes to meet a female 
aged between 24-29 inclusive; his interests are movies, tennis, walking and computers. 
Write the code to process the client list, assumed to be in a file named clients.txt into a 
dictionary called clients. The name of the client is the dictionary key which you can assume to 
be unique and the remaining client information i.e. the dictionary value should be a list.  
Clients are compatible if each one is of the gender and age range that the other is seeking. 
For the purposes of this question you can ignore common interests. No-one should be matched to themselves.  
Write the code to a function check_match that accepts a client’s name as a string, determines suitable matches 
and outputs the matches to the screen e.g. assuming the client was Alison Jones, potential matches would be 
John Smith, Brian Adams and Chris Jones. 
Alison Jones should meet John Smith. Alison Jones should meet Brian Adams. Alison Jones should meet Chris Jones. 
