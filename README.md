# Coffee-machine
This is a simple coffee machine programme
This code is a Python script for a simple coffee machine simulation. Let's break down what each part does:

Imports:

from menu import Menu: Imports the Menu class, which presumably contains the menu options for the coffee machine.
from coffee_maker import CoffeeMaker: Imports the CoffeeMaker class, which represents the coffee maker itself and handles making coffee and checking resources.
from money_machine import MoneyMachine: Imports the MoneyMachine class, which handles transactions and money-related operations.
Initialization:

is_on = True: Initializes a boolean variable is_on to control whether the coffee machine is running.
Object Instantiation:

coffee_maker = CoffeeMaker(): Instantiates a CoffeeMaker object.
money_machine = MoneyMachine(): Instantiates a MoneyMachine object.
menu = Menu(): Instantiates a Menu object.
Main Loop:

The while loop runs as long as is_on is True.
Inside the loop, it prompts the user to choose an item from the menu by calling menu.get_items().
If the user enters "off", it sets is_on to False, exiting the loop and turning off the coffee machine.
If the user enters "report", it calls coffee_maker.report() and money_machine.report() to print reports about the resources and money status.
Otherwise, it assumes the user has chosen a drink. It uses menu.find_drink(choice) to get the Drink object corresponding to the user's choice.
It then checks if there are sufficient resources using coffee_maker.is_resource_sufficient(drink). If there are, it proceeds to payment.
It uses money_machine.make_payment(drink.cost) to process the payment. If the payment is successful, it makes the coffee using coffee_maker.make_coffee(drink).
Overall, this code simulates a basic coffee machine operation where users can choose drinks from a menu, check the machine's status, and turn it off when needed.
