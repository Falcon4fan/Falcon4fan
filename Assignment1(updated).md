#Program tests all thirteen password conditions
#The passwords must be in the format <part-1>#<part-2>
#The <part-1> consists of only alphanumeric characters or dot ‘.’
#The dot ‘.’ cannot be the first or last character in <part-1> and it cannot appear consecutively
#The <part-2> only consists of alphanumeric characters and no character is to be repeated within <part-2>.

#For first password abc#abc

SpecialSym = ('.', '#')

ap1 = "abc"

if (ap1[0:1] == '.' or ap1[1:2] == '.'):
    print("abc#abc is invalid")

ap2 = "abc"  

for x in ap2:
     x = 0
        
if x > 1:
    print("abc#abc is invalid")
else:
    print("abc#abc is valid")
    
pw1 = ap1 + '#' + ap2


#For second password 1#patch
ap3 = "1"

if (ap3[0:1] == '.' or ap3[1:2] == '.'):
    print("1#patch is invalid")

ap4 = "patch"  

for x in ap4:
     x = 0
        
if x > 1:
    print("1#patch is invalid")
else:
    print("1#patch is valid")
    
pw2 = ap3 + '#' + ap4


#For third password a.b#cd9

ap5 = "a.b"

if (ap5[0:1] == '.' or ap5[2] == '.'):
    print("a.b#cd9 is invalid")

ap6 = "cd9"  

for x in ap6:
     x = 0
        
if x > 1:
    print("a.b#cd9 is invalid")
else:
    print("a.b#cd9 is valid")
    
pw3 = ap5 + '#' + ap6


#For fourth password 12to13#timesup

ap7 = "12to13"

if (ap1[0:1] == '.' or ap1[1:2] == '.'):
    print("12to13#timesup is invalid")

ap8 = "timesup"  

for x in ap8:
     x = 0
        
if x > 1:
    print("12to13#timesup is invalid")
else:
    print("12to13#timesup is valid")
    
pw4 = ap7 + '#' + ap8


#For fifth password a.b.c#987 is valid

ap9 = "a.b.c"

if (ap1[0:1] == '.' or ap1[1:2] == '.'):
    print("12to13#timesup is invalid")

ap10 = "987"  

for x in ap10:
     x = 0
        
if x > 1:
    print("a.b.c#987 is invalid")
else:
    print("a.b.c#987 is valid")
    
pw5 = ap9 + '#' + ap10


#For sixth password .ab#123 is valid
 
ap11 = ".ab"

if (ap11[0] == '.' or ap11[2] == '.'):
    print(".ab#123 is invalid")

ap12 = "123"  

for x in ap12:
     x = 0
        
if x > 1:
    print(".ab#123 is invalid")
else:
    print(".ab#123 is valid")
    
pw6 = ap11 + '#' + ap12


#For seventh password .ab#123 is valid
