# Ex-Chapter-3
## Exercise 1

import random
fortune_cookie_1="Love, because it is the only true adventure."
fortune_cookie_2="Enjoy yourself, it's latter than you think."
fortune_cookie_3="Your road to glory will be rocky, but fulfilling."
fortune_cookie_4="Nothing is so much to be feared as fear."
fortune_cookie_5="All things are diffiult before yhey are easy."

print("\nYour fortune cookie says: \n")
fort_numb=random.randint(1,5)
if fort_numb==1:
    print(fortune_cookie_1)
elif fort_numb==2:
    print(fortune_cookie_2)
elif fort_numb==3:
    print(fortune_cookie_3)
elif fort_numb==4:
    print(fortune_cookie_4)
else:
    print(fortune_cookie_5)


## Exercise 2 

count_number = 1
heads_value = 0
tails_value = 0
while count_number <= 100:
    coin_value= random.randint(1,2)
    count_number+=1
    if coin_value==1:
        heads_value+=1
    elif coin_value==2:
        tails_value+=1
    else:
        print('The coin does not have head or tail.')

print("After flipping the coin 100 times:" ,heads_value,"times heads and" ,tails_value,"times tails.\n\n")


## Exercise 3

number = random.randint(1,50)
guess_number = int(input('Pick a number:'))
guess_tries = 1

while guess_number != number:
    guess_tries+=1
    if guess_tries > 5 :
        print('Failed! you wasted 5 attempts.\n')
        break
    elif guess_number > number:
        print('Try again, too higher')
    else:
        print('Try again, too lower')
    guess_number = int(input('Pick a number:'))

if guess_number == number:
    print('You guessed it! the number was',number)

    
## Exercise 4 

#Let the player pick a guess number (int(input()))
#Let the computer pick a random number between 1-10 (random.randint(1,10))
#Set the guess tries to 1 (tries = 1)
#While random number is not equal to the player number 
#Increase the guess tries by 1
#Set another random number between 1-10
#If the computer random number is equal to the player number , let the player know , and how many tries it took 
#End the game 
