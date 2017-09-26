import random
import game_functions

PITCH_WIDTH = 50
PITCH_LENGTH = 100
time_elapsed = 0.0
TOTAL_TIME = 90
location = [50, 25]
score = [0, 0]
type_of_move = ""
mode = ""
help_page = "This is the help page. Please always follow the instructions that follow the question and you should be fine!"
one_two = 0
have_ball = True

print("Welcome to Dylan's texted based FIFA game!")
help_page_wanted = game_functions.getBool(input("Would you like the help page? (Please enter 'Yes' or 'No')"))
while help_page_wanted != False and help_page_wanted != True:
    help_page_wanted = game_functions.getBool(input("Would you like the help page? (Please enter 'Yes' or 'No')"))
if help_page_wanted == True:
    print(help_page)
while one_two != 1 and one_two != 2:
    one_two = int(input("Would you like to play single or two player? (Enter 1 or 2)"))

if one_two == 1:
    print("\nYou have chosen the one-player game. You will be playing against the com.")
    heads = input("\nWould you like heads or tails(Enter 'heads' or 'tails')")
    while heads != "heads" and heads != "tails":
        heads = input("Would you like heads or tails(Enter 'heads' or 'tails')")
    if heads == "heads":
        heads = 1
    else:
        heads = 2
    kick_off = random.randint(1,2)
    if kick_off == heads:
        print("You won the toss! You will start.")
        mode = "Attack"
    else:
        print("You lost the toss! The com will start.")
        mode = "Defend"
    print("\n\nKick off!")
    while time_elapsed != TOTAL_TIME:
        time_elapsed = time_elapsed + 1
        if mode == "Attack":
            type_of_move = input("What attacking move would you like to play? (Enter 'pass', 'dribble', or 'shoot')")
            while type_of_move != "pass" and "dribble" and "shoot":
                type_of_move = input("What attacking move would you like to play? (Enter 'pass', 'dribble', or 'shoot')")
            if type_of_move == "pass":
                game_functions.passing()


