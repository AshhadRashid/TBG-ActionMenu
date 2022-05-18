# TBG-ActionMenu
#TBG Action Menu - Muhammad Rashid
#May 17, 2022
#This code is an action menu for my TBG. The code will be the startup
#to the TBG.

#actions list
actions = ['Attack','Dodge','Heal']

#consumables list
consumables = ['Mushroom','Fire Flower','Star']                                         
print('Welcome to the Super Mario Bros Text Based Game!\n')
print('Choose one of the following actions:')

#for loop to print all items in actions list
for action in actions:                                                                   
    print('* ' + action)
useraction = input()

#if user picks attack it will print a message
if useraction == 'Attack':                                                              
    print('\nYour attack dealt 20 damage points')
    
#if user picks dodge it will print a message   
elif useraction == 'Dodge':                                                             
    print('\nYou have succesfully evaded the attack')
    
#if user picks heal it will print a message     
elif useraction == 'Heal':                                                              
    print('\nWhich consumable would you like to heal with?')
    for consumable in consumables:                                                      
        print('* ' + consumable)
    healchoice = input()
    if healchoice == 'Mushroom':
        print('\nYou have gained 50 health points')
    elif healchoice == 'Fire Flower':
        print('\nYou have gained 100 health points')
    elif healchoice == 'Star':
        print('\nYou have become invincibile for a short period of time')
    else:
        print('That is not a valid option')
#if user types incorrectly the program will detect it
else:
    print('That is not a valid option')
    
