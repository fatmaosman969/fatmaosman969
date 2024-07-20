import time

def print_pause(text, delay=2):
    print(text)
    time.sleep(delay)

def start_game():
    print_pause("Welcome to the adventure game!", 2)
    print_pause("You are in a house haunted by ghosts. You have two options: '1' to exit or '2' to explore.", 2)
    user_input = input("What do you want to do? ").lower()
    
    if user_input == '1':
        print("I'm out of the game. Thanks for playing!")
    elif user_input == '2':
        explore_room()     
    else:
        print("Invalid selection. Try again.")
        start_game()

def explore_room():
    print_pause("You are now in a room full of treasures!", 2)
    print_pause("You can choose '1' to take the treasure or '2' to return.", 2)
    
    user_input = input("What do you want to do? ").lower()
    
    if user_input == '1':
        print("You took the treasure! Congratulations!")
        # يمكنك إضافة المزيد من المنطق هنا مثل زيادة النقاط أو إنهاء اللعبة
    elif user_input == '2':
        start_game()  # العودة إلى بداية اللعبة
    else:
        print("Invalid selection. Try again.")
        explore_room()  # إعادة الطلب من المستخدم

# بدء اللعبة
start_game()
def explore_room():
    print_pause("You are now in a room full of treasures!", 2)
    print_pause("You can choose '1' to take the treasure, '2' to return, or '3' to face the ghost.", 2)
    
    user_input = input("What do you want to do? ").lower()
    
    if user_input == '1':
        print("You took the treasure! Congratulations!")
    elif user_input == '2':
        start_game()  # العودة إلى بداية اللعبة
    elif user_input == '3':
        print("You bravely face the ghost! But it scares you away...")
        start_game()  # العودة إلى بداية اللعبة
    else:
        print("Invalid selection. Try again.")
        explore_room()  # إعادة الطلب من المستخدلة لمساعدتك:

