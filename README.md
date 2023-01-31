# rock-Scissor-paper

import random              
possibilities=['rock','scissor','paper']
game_choice=input('do you want to play? yes/no')
while(game_choice=='yes'):
    userInput=input('enter rock/scissor/paper ')
    num1 = random.randint(0, 2)
    comp_choice=possibilities[num1]
    while (comp_choice==userInput):
        num1 = random.randint(0, 2)
        comp_choice=possibilities[num1]
    print("computer choice is ",comp_choice)    
    if (userInput=='rock' and comp_choice=='paper'):
        print('Computer is Lucky! Paper win')
    elif (userInput=='paper' and comp_choice=='rock'):
        print('You are Lucky! Paper Win')
    elif (userInput=='rock' and comp_choice=='scissor'):  
        print('You are Lucky! Rock Win')
    elif (userInput=='scissor' and comp_choice=='rock'):  
        print('computer is Lucky! rock Win')   
    elif (userInput=='paper' and comp_choice=='scissor'):
        print('computer is Lucky! Scissor Win')   
    elif (userInput=='scissor' and comp_choice=='paper'):
        print('You are Lucky! Scissor Win') 
     
    game_choice=input('do you want to play? yes/no')
