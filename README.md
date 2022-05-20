# 19-05-22-ass-2
from math import sqrt 
def checkprime(numberTocheck):
     if numberTocheck==1:
        return False
     for i in range(2,int(sqrt(numberTocheck))+1):
         if numberTocheck%i==0:
            return False
     return True
def primeSum(l,r):
   sum=0
   for i in range(r,(l-1),-1):
       isPrime=checkPrime(i)
       if(isPrime):
           sum+=i
   return sum
   
if_name=="__main__":
   l,r=4,13
   print(printSum(l,r))
   
output:
36
