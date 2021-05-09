#Program tests all thirteen password conditions
#The passwords must be in the format <part-1>#<part-2>
#The <part-1> consists of only alphanumeric characters or dot ‘.’
#The dot ‘.’ cannot be the first or last character in <part-1> and it cannot appear consecutively
#The <part-2> only consists of alphanumeric characters and no character is to be repeated within <part-2>.

#For first password abc#abc

SpecialSym = (".","#")

ap1 = "abc"

if (ap1[0,1] == "." or ap1[1,2] == "."):
    print("abc#abc is invalid")

ap2 = "abc"  

for x in ap2:
     x = 0
        
if x > 1:
    print("abc#abc is invalid")
else:
    continue
    
pw1 = ap1 + '#' + ap2

print(pw1)
