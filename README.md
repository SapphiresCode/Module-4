# Module-4
school project, python code

# Copy the code from line 6 into a python code viewer

import time #do NOT delete this
#the printed '' allows for there to be numerous lines of no text
#   and as a result, a far cleaner look when starting up the program, 
#       pushing any python start script upwards 24 lines
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('') #formatting
print('----------------------') #formatting, border for the title
#the title, yeah it's fancy and unneeded, but it's fun and it makes it stand out (and look better too)
time.sleep(0.5)#formatting, visual effect
print("  ____  _____  _____ _  __ __      __     _     _    _ ______ ") #title 
time.sleep(0.5)#formatting, visual effect
print(" |  _ \|  __ \|_   _| |/ / \ \    / /\   | |   | |  | |  ____|") #title 
time.sleep(0.5)#formatting, visual effect
print(" | |_) | |__) | | | | ' /   \ \  / /  \  | |   | |  | | |__   ") #title 
time.sleep(0.5)#formatting, visual effect
print(" |  _ <|  _  /  | | |  <     \ \/ / /\ \ | |   | |  | |  __|  ") #title 
time.sleep(0.5)#formatting, visual effect
print(" | |_) | | \ \ _| |_| . \     \  / ____ \| |___| |__| | |____ ") #title 
time.sleep(0.5)#formatting, visual effect
print(" |____/|_|  \_\_____|_|\_\     \/_/    \_\______\____/|______|") #title 
time.sleep(0.5)#formatting, visual effect
print("                                                              ") #title  
time.sleep(0.5)#formatting, visual effect
print("   _____          _      _____ _    _ _            _______ ____  _____  ") #title  
time.sleep(0.5)#formatting, visual effect
print("  / ____|   /\   | |    / ____| |  | | |        /\|__   __/ __ \|  __ \ ") #title  
time.sleep(0.5)#formatting, visual effect
print(" | |       /  \  | |   | |    | |  | | |       /  \  | | | |  | | |__) |") #title  
time.sleep(0.5)#formatting, visual effect
print(" | |      / /\ \ | |   | |    | |  | | |      / /\ \ | | | |  | |  _  / ") #title  
time.sleep(0.5)#formatting, visual effect
print(" | |____ / ____ \| |___| |____| |__| | |____ / ____ \| | | |__| | | \ \ ") #title  
time.sleep(0.5)#formatting, visual effect
print("  \_____/_/    \_\______\_____|\____/|______/_/    \_\_|  \____/|_|  \_\ ") #title
time.sleep(0.5)#formatting, visual effect
print("                                                                        ") #title                        
time.sleep(0.5)#formatting, visual effect
#the time.sleep function is used for two purposes, in the title (purely for visual effect)
#   and functionally when data is being spat back out at the user so then the user has
#       time to read what is being said before the next data is printed.
#the time.sleep is set and 0.5 which means it takes half a second for the next bit of data to appear
#   in other words, the title takes 6.5 seconds to "load" due to 14 time.sleep functions being used. 
#       time.sleep functions marked with "visual effect" can be removed with no issues, due to serving no
#           functional purpose, time.sleep functions marked with "functional effect" should not be removed
#               for user usability as without, it would make the program a lot less user friendly.
print('----------------------') #formatting, border for the title
print('Supabriks 2025') #formatting, visual effect
print('') #formatting
time.sleep(0.5)#formatting, visual effect
time.sleep(0.5)#formatting, visual effect
print('') #formatting
print('') #formatting

#creates a "Brik" class
class Brik:
    name = "Brik"
    #length holds int
    #width holds int
    #height holds int

    def __init__(self, length, width, height):
        self.length = length
        self.width = width
        self.height = height

    def GetName(self): #Name
        return self.name 
    
    def GetLength(self): #Length
        return self.length
    
    def GetWidth(self): #Width
        return self.width
    
    def GetHeight(self): #Height
        return self.height

#catagory, finding out which brik type will be used
catagory = input("Enter the category of brik. (t = tall, f= flat, s= SupaFig) > ")

#tall class (Brik)
if catagory is ("t"):
    class Brik:
        name = "Brik"
        #length holds int
        #width holds int
        #height holds int

        length = int(input("Enter the length in units. > ")) #Enter Length
        width = int(input("Enter the width in units. > ")) #Enter Width
        height = int(input("Enter the height in units. > ")) #Enter Height
        base = width * length
        value = base * 0.1 
        value2 = value + height * 0.2
        def __init__(self, length, width, height):
        
            self.length = length
            self.width = width
            self.height = height

        def GetName(self):
            return self.name
    
        def GetLength(self):
            return self.length
    
        def GetWidth(self):
            return self.width
    
        def GetHeight(self):
            return self.height
        print('') #formatting
        print("Your brik: Tall")
        time.sleep(0.5)#formatting, functional effect
        print('') #formatting
        print(f"DIMENSIONS: length of {length}, width of {width}, height of {height}")
        print('') #formatting
        time.sleep(0.5)#formatting, functional effect
        print(f"PREDICTED MARKET VALUE: ${value2}")
        print('') #formatting
       
#Flat class, overwrites init  
if catagory is ("f"):     
    class Flat(Brik):
        length = int(input("Enter the length in units. > ")) #Enter Length
        width = int(input("Enter the width in units. > ")) #Enter Width
        height = int(0)
        def __init__(self, length, width, height):
            self.name = "Flat Brik"
            self.width = width
            self.height = height
            self.length = length
        getcost = width * length * 0.15
        print("Your brik: Flat")
        time.sleep(0.5)#formatting, functional effect
        print('') #formatting
        print(f"DIMENSIONS: length of {length}, width of {width}, height of 0")
        print('') #formatting
        time.sleep(0.5)#formatting, functional effect
        print(f"PREDICTED MARKET VALUE: ${getcost}")
        print('') #formatting
        
#SupaFig class, overwrites init
if catagory is ("s"):
    class SupaFig(Brik):
        def __init__(self, length, width, height, getcost):
            self.name = "SupaFig"
            length = int(2)
            width = int(1)
            height = int(3)
            cost = int(2.85)
            self.width = width
            self.height = height
            self.length = length
            self.getcost = cost
        print('') #formatting
        print("Your brik: SupaFig")
        print('') #formatting
        time.sleep(0.5)#formatting, functional effect
        print(f"DIMENSIONS: length of 2, width of 1, height of 3")
        print('') #formatting
        time.sleep(0.5)#formatting, functional effect
        print(f"PREDICTED MARKET VALUE: $2.85")
        print('') #formatting

#============================= Notes =============================
# This section is dedicated towards notes taken during development
#=================================================================
# 
# Tkinter software *still* does not work on my computer, so I was
#   unable to make the program run in a GUI, however when I was made
#       aware of this, I had already constucted a basic version of the
#           program (module 4.py), and decided to combine that version with
#               the layout from the task "fruitStore" to attempt to at least get
#                   the calculator section functional, while it does still run in
#                       python terminal opposed to a new window, it still fufills the task
#                           requirements as asked (in fact- better if you consider requirement 3)
#
# Session 1 - module 4 creation 14/5/25
# Session 2 - module 4-2 creation 15/5/25
# Session 3 - comments, cat testing document and visual effects - 19/5/25
#
#        _            _                   _          _          _       _     _          _           _      
#       / /\         / /\                /\ \       /\ \       / /\    / /\  /\ \       /\ \        /\ \    
#      / /  \       / /  \              /  \ \     /  \ \     / / /   / / /  \ \ \     /  \ \      /  \ \   
#     / / /\ \__   / / /\ \            / /\ \ \   / /\ \ \   / /_/   / / /   /\ \_\   / /\ \ \    / /\ \ \  
#    / / /\ \___\ / / /\ \ \          / / /\ \_\ / / /\ \_\ / /\ \__/ / /   / /\/_/  / / /\ \_\  / / /\ \_\ 
#    \ \ \ \/___// / /  \ \ \        / / /_/ / // / /_/ / // /\ \___\/ /   / / /    / / /_/ / / / /_/_ \/_/ 
#     \ \ \     / / /___/ /\ \      / / /__\/ // / /__\/ // / /\/___/ /   / / /    / / /__\/ / / /____/\    
# _    \ \ \   / / /_____/ /\ \    / / /_____// / /_____// / /   / / /   / / /    / / /_____/ / /\____\/    
#/_/\__/ / /  / /_________/\ \ \  / / /      / / /      / / /   / / /___/ / /__  / / /\ \ \  / / /______    
#\ \/___/ /  / / /_       __\ \_\/ / /      / / /      / / /   / / //\__\/_/___\/ / /  \ \ \/ / /_______\   
# \_____\/   \_\___\     /____/_/\/_/       \/_/       \/_/    \/_/ \/_________/\/_/    \_\/\/__________/   
