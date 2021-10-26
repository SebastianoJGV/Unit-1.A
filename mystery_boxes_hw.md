'''
Created on Sep. 17, 2021

@author: sebas
'''
'''.py
import math

#mysterybox1 reverses a string, and if true makes is all lower case
def mysterybox1(stringinput, n):
    x=stringinput
    if n == 1:
        x=stringinput.lower()
        print(x[::-1])
    else:
        return print(x[::-1])
    
mysterybox1("Hello", False)
     
#Mysterybox2 seperates a email into the first name and @gmail.com or so on

def mysterybox2(i):
    n=i.find("@")
    print(i[0:(n)])
    return print(i[n:])

mysterybox2("johndoe@gmail.com")

# mystery box 3 finds the lowest common multiple

def mysterybox3(a):
    lcm = a[0] 
    for i in range(1,len(a)):
        lcm = lcm*a[i]//math.gcd(lcm, a[i])
    return print(lcm)


lisa = [8, 2, 1]
mysterybox3(lisa)

# mystery box 4 takes a list, removes the two biggest items, then calcualtes a new average and prints a new version of the list

def mysterybox4(inp):
    inp.sort()
    boom = inp[0:-2]
    return print(f"{sum(boom)/len(boom)}, {boom}")
x = [5, 6, 3, 8, 1, 7, 9]
mysterybox4(x)
'''

