# Strategy of playing to win the game :
'''
Avoid the uni-digit (Last Digit) of the resulted number of calculation.
That's the gotten number.
'''

# Code of the game:

import numpy as np 

number=np.random.randint(1,100)
QS=f'''
I'm Thinking about a number between 1 to 100.
I multiply that number by 2.
Then, add 2 with that.
After that,I multiply the gotten result with 5 again.
At last, I substract 6 from that.
I get finally 
'''

def n(number):
    num=number
    num*=2
    num+=2
    num*=5
    num-=6
    Ask=int(input(f"{QS} {num}\nCan you guess the number, that I was thinking?"))
    if Ask==number:
        print("Oh you're correct!")
    else :
        print(f"Sorry, the number is {number}")
        

n(number)


