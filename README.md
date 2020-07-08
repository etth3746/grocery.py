# grocery.py

#This code runs a simple grocery game where a menu is displayed to the user and that user must decide what to buy to complete the grocery list
#Author: Ethan Thompson

def rules():

    print("The goal of this game is to shop at the Python grocery store in order to complete the grocery list.")
    print("Once the list is empty, the game is over.")
    print("There is no time limit, just have fun trying to find your way around the store!\n")
    grocery_list = ['Apples', 'Bananas', 'Ice Cream', 'Steak', 'Milk', 'Bread'] 
    store(grocery_list)



def store(grocery_list):

    if grocery_list == []:      #If the list is empty print 'Game Over'
            gameEnd()


    print("---Directory---")        #Prints directory of departments in the store
    print("Dry Goods")
    print("Meat")
    print("Frozen")
    print("Dairy")
    print("Toys")
    print("Electronics")
    print("Apparel")
    print("Deli")
    print("Produce")

    department_choice = input("\nWhich department would you like to go to?\n").upper()
       

    if department_choice == "DRY GOODS":                                             #If user wants to go to dry goods
        print("\nHere are all of the items located in Dry Goods:\n")
        items_in_dry = ['Bread', 'Chips', 'Sugar', 'Skittles', 'Rolos', 'Lucky Charms', 'Donuts', 'Root Beer']      #A list of all items located in this department
        for items in items_in_dry:
            print(items)

        need = input("\nWhat do you need from this department? If you don't need anything from this area please enter 'Go Back'\n")

        if need == "Go Back":
            store(grocery_list)
        
        elif need in grocery_list:
            
            grocery_list.remove(need)
            print(need + " was removed from the list. Here is your current list:\n")
            print(grocery_list)
            
            store(grocery_list)

        else:
            print( need + " is not on the list\n")
            store(grocery_list)
        

        

    elif department_choice == "MEAT":                   #If the user wants to go to Meat
        print("\nHere are the items located in Meat:\n")
        items_in_meat = ["Steak", "T-bone", "Burgers", "Chicken Breast"]        #A list of all items located in this department
        for items in items_in_meat:
            print(items)

        need = input("\nWhat do you need from this department? If you don't need anything from this department please enter 'Go Back'\n")

        if need == "Go Back":
            store(grocery_list)

        elif need in grocery_list:
            grocery_list.remove(need)
            print(need + " was removed from the list. Here is your current list:\n")
            print(grocery_list)
            store(grocery_list)

        else:
            print(need + " is not on the list\n")
            store(grocery_list)


    
    
    elif department_choice == "FROZEN":                     #If the user wants to go to Frozen
        print("\nHere are the items located in Frozen:\n")
        items_in_frozen = ["Frozen Chicken", "Toaster Strudel", "Eggo Waffles", "Ice Cream", "Frozen Veggies"]      #A list of all items located in this department
        for items in items_in_frozen:
            print(items)


        need = input("\nWhat do you need from this department? If you don't need anything from this department please enter 'Go Back'\n")

        if need == "Go Back":
            store(grocery_list)

        elif need in grocery_list:
            grocery_list.remove(need)
            print(need + " was removed from the list. Here is your current list:\n")
            print(grocery_list)
            store(grocery_list)

        else:
            print(need + " is not on the list\n")
            store(grocery_list)



    elif department_choice == "DAIRY":                      #If the user wants to go to Dairy
        print("\nHere are the items located in Dairy:\n")
        items_in_dairy = ["Milk", "Eggs", "Yogurt", "Cheese", "Butter"]         #A list of all items located in this department
        for items in items_in_dairy:
            print(items)

        
        need = input("\nWhat do you need from this department? If you don't need anything from this department please enter 'Go Back'\n")

        if need == "Go Back":
            store(grocery_list)

        elif need in grocery_list:
            grocery_list.remove(need)
            print(need + " was removed from the list. Here is your current list:\n")
            print(grocery_list)
            store(grocery_list)

        else:
            print(need + " is not on the list\n")
            store(grocery_list)

            

    elif department_choice == "TOYS":                          #If the user wants to go Toys
        print("\nHere are all the items located in Toys:\n")
        items_in_toys = ["Lego Set", "Nerf Gun", "Barbie", "Board Game", "Puzzle"]      #A list of all items located in this department
        for items in items_in_toys:
            print(items)

        
        need = input("\nWhat do you need from this department? If you don't need anything from this department please enter 'Go Back'\n")

        if need == "Go Back":
            store(grocery_list)

        elif need in grocery_list:
            grocery_list.remove(need)
            print(need + " was removed from the list. Here is your current list:\n")
            print(grocery_list)
            store(grocery_list)

        else:
            print(need + " is not on the list\n")
            store(grocery_list)



    elif department_choice == "ELECTRONICS":                        #If the user wants to go to Electronics
        print("\nHere are all the items located in Electronics:\n")
        items_in_electronics = ["Samsung 50' TV", "Bose Soundbar", "PS5", "Acer Monitor", "Sony Headphones"]        #A list of all items located in this department
        for items in items_in_electronics:
            print(items)

        need = input("\nWhat do you need from this department? If you don't need anything from this department please enter 'Go Back'\n")

        if need == "Go Back":
            store(grocery_list)

        elif need in grocery_list:
            grocery_list.remove(need)
            print(need + " was removed from the list. Here is your current list:\n")
            print(grocery_list)
            store(grocery_list)

        else:
            print(need + " is not on the list\n")
            store(grocery_list)



    elif department_choice == "APPAREL":                               #If the user wants to go to Apparel
        print("\nHere are all of the items located in Apparel:\n")
        items_in_apparel = ["Supreme Hoodie", "Gucci Sunglasses", "Louis Vuitton Handbag", "Patagonia T-Shirt"]     #A list of all items located in this department
        for items in items_in_apparel:
            print(items)


        need = input("\nWhat do you need from this department? If you don't need anything from this department please enter 'Go Back'\n")

        if need == "Go Back":
            store(grocery_list)

        elif need in grocery_list:
            grocery_list.remove(need)
            print(need + " was removed from the list. Here is your current list:\n")
            print(grocery_list)
            store(grocery_list)


        else:
            print(need + " is not on the list\n")
            store(grocery_list)
        


    elif department_choice == "DELI":                           #IF the user wants to go to Deli
        print("\nHere are all of the items located in Deli\n")
        items_in_deli = ["Bread", "Sliced Ham", "Sliced Cheese", "Pepperoni", "Salami"]     #A list of all items located in this department
        for items in items_in_deli:
            print(items)


        need = input("\nWhat do you need from this department? If you don't need anything from this department please enter 'Go Back'\n")

        if need == "Go Back":
            store(grocery_list)

        elif need in grocery_list:
            grocery_list.remove(need)
            print(need + " was removed from the list. Here is your current list:\n")
            print(grocery_list)
            store(grocery_list)

        else:
            print(need + " is not on the list\n")
            store(grocery_list)




    elif department_choice == "PRODUCE":                            #If the user wants to go to Produce
        print("\nHere are all of the items located in Produce:\n")
        items_in_produce = ["Apples", "Bananas", "Peaches", "Strawberries", "Watermelon"]       #A list of all items located in this department
        for items in items_in_produce:
            print(items)


        need = input("\nWhat do you need from this department? If you don't need anything from this department please enter 'Go Back'\n")

        if need == "Go Back":
            store(grocery_list)

        elif need in grocery_list:
            grocery_list.remove(need)
            print(need + " was removed from the list. Here is your current list:\n")
            print(grocery_list)
            store(grocery_list)


        else:
            print(need + " is not on the list\n")
            store(grocery_list)



    
        



def main():

    print("Welcome to Grocery! This game is all about completing the grocery list by shopping around the store.")
    first_time = input("Is this your first time playing?\n").upper()


    if first_time == "YES":
        print("\nWelcome newcomer! Here are the rules:\n")
        rules()

    elif first_time == "NO":
        rules_answer = input("Welcome back! Would you like to hear the rules?\n").upper()

        if rules_answer == "YES":
            rules()

        elif rules_answer == "NO":
            print("\nGreat! Have fun!\n")
            grocery_list = ['Apples', 'Bananas', 'Ice Cream', 'Steak', 'Milk', 'Bread'] 
            store(grocery_list)

    else:

        print("Please enter either 'Yes' or 'No'")
    


def gameEnd():

    play_again = input("\nYour list is empty! Would you like to play again?\n").upper()

    if play_again == "YES":
            main()

    else:

        print("Game Over. Thank you for playing\n")
    



main()






