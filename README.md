# sr-flipflop
SR 

def AND(a,b,c): 
 return a&b&c
 
def OR(a,b): 
 return a|b
 GitHub link :- click
def NOT (a):
 return int(not a)
def NOR(a,b): 
 ans = OR(a,b)
 return NOT(ans)
S = int(input())
R = int(input())
Qp = int(input("Previous"))
a1 = AND(R,1,1)
a2 = AND(S,1,1)
if(a1 == a2 == 1):
 print(" Intermediate")
else:
 a3 = NOR(a2,Qp)
 Qn = NOR(a1,a3)
 print("value of Next Output is = ",Qn)
