from fractions import Fraction
from decimal import Decimal
import struct, socket, time, math, array, re, sys, os

a = int(raw_input("Enter the value for A:"))
b = int(raw_input("Enter the value for B:"))
c = int(raw_input("Enter the value for C:"))

if int(a) == 0 :
    print "The value of A cannot be 0."
    
#Check 1----------------------------------------------
def discriminant(a,b,c):
    try:
       math.sqrt(b*b-4*a*c)
    except ValueError:
        print "\n\n\n\nThe given expression cannot be factored.\n\nDiscriminant is negative, equation has no real solutions, only 2 complex solutions."
        sys.exit("Read reason for exit above.")

#Calculation result using the cuadratic formula----------------
def cuadratic(a,b,c,sign):
    int(a)
    int(b)
    int(c)
    bool(sign)
    
    if sign == True : 
            nume = ((-1 * b) + math.sqrt(b*b - 4*a*c))
            deno = (2*a)
            X1 = Fraction(int(nume), deno)
            return (((-1 * b) + math.sqrt(b*b-4*a*c)) / (2*a))
    else :
            nume = ((-1 * b) - math.sqrt(b*b - 4*a*c))
            deno = (2*a)
            X2 = Fraction(int(nume), deno)
            return (((-1 * b) - math.sqrt(b*b - 4*a*c)) / (2*a))


discriminant(a,b,c)
x1 = cuadratic(a,b,c,True)
x2 = cuadratic(a,b,c,False)

def display(x1, x2) :
    print "\n The factorization is: "
    print "\n (x",
    if x1 < 0 :
        x1 = x1*-1
        print "+", x1,
    else :
        print "-", x1,
    print ')(x',
    if x2 < 0 :
        x2 = x2*-1
        print "+", x2,
    else :
        print "-", x2,  	
    print ")"

display(x1, x2)

##End of program---------------------------------------------------------------------------
##Check 1----------------------------------------------Not really neccesary, at this moment
##def rationalization(a,b,c):
##    x = math.sqrt(b*b-4*a*c)
##    if float(x) != int(x):
##                        print "Float x is not an int"
##                        return False
##    else :
##                        return True
##rationalization(a,b,c)
    
