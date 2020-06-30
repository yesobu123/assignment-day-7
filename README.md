Assignment 1:                                                                                                                                                                  
#import module sys to get the type of exception                                                                                                                 
import sys                                                                                                                                             
randomList = ['a', 0, 2]
for entry in randomList:                                                                                                                                                   
    try:                                                                                                                                                                  
        print("The entry is", entry)                                                                                                                                    
        r = 1/int(entry)                                                                                                                                              
        break                                                                                                                                                      
    except:                                                                                                                                                                    
        print("Oops!", sys.exc_info()[0], "occurred.")                                                                                                                    
        print("Next entry.")                                                                                                                                               
        print()                                                                                                                                                         
print("The reciprocal of", entry, "is", r)  
                                                                                                                                                                           
OUTPUT:                                                                                                                                                               
The entry is a                                                                                                                                       
Oops! <class 'ValueError'> occurred.                                                                                                                          
Next entry.                                                                                                                                                         
The entry is 0                                                                                                                                                                
Oops! <class 'ZeroDivisionError'> occured.                                                                                                                                
Next entry.                                                                                                                                                             
The entry is 2                                                                                                                                                                
The reciprocal of 2 is 0.5                                                                                                                                                  
                                                                                                                                                                             
Assignment 2:                                                                                                                                                                   
  def test_prime(n):                                                                                                                                                       
    if (n==1):                                                                                                                                                           
       return False                                                                                                                                                           
     elif (n==2):                                                                                                                                                      
       return True;                                                                                                                                     
    else:                                                                                                                                                                 
        for x in range(2,n):                                                                                                                                           
          if(n % x==0):                                                                                                                                                   
              return False                                                                                                                                                      
            return True             
print(test_prime(9))                                                                                                                                                   
                                                                                                                                                                      
OUTPUT:                                                                                            
FALSE                                                                           
