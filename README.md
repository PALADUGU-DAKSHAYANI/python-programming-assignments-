# python-programming-assignments-
python programme to check whether a number can be written as sum of three perfect squares or not

PROGRAMME:
#threesquares method 
def threesquares(m):
    a=0
    b=0
    flag=1
    while(a>=0 and flag!=0):
         if((4**a)*(7)>m):
              break
         while(b>=0 and ((4**a)*((8*b)+7))<=m):
                  if((4**a)*((8*b)+7)==m):
                      print(a)
                      print(b)
                      flag=0
                      break
                  else:
                      b=b+1 
         b=0
         a=a+1
    if(flag==1):
        return True 
    else:
        return False
        
n=int(input())
print(threesquares(n))
    
