# CoffeeMachine

This code defines a coffee machine menu and simulates a coffee order process, where the user can choose a drink, insert coins to pay for it, and get the drink with any necessary change.

The menu is defined as a dictionary called MENU that contains three coffee types (espresso, latte, and cappuccino). Each coffee type has a nested dictionary that contains the required ingredients and their amounts, as well as the cost of the drink.

The code also defines two additional dictionaries: resources, which contains the initial stock of ingredients available in the machine, and profit, which keeps track of the total amount of money made from successful transactions.

The coffee order process is simulated using a while loop that runs as long as is_on is True. The user is prompted to choose a drink from the menu or enter off to turn off the machine. If the user enters report, the current stock of ingredients and total profit are printed.

If the user chooses a coffee type, the code checks if there are enough resources to make the drink by calling the is_resource_sufficient function. If there are enough resources, the code prompts the user to insert coins by calling the process_coins function. The function calculates the total amount of money inserted and returns it.

The total payment is then checked against the cost of the drink by calling the is_transaction_successful function. If the payment is sufficient, the necessary ingredients are deducted from the resources dictionary by calling the make_coffee function, which also prints a message to indicate that the drink is ready.

If the payment is insufficient, the user is prompted to insert more coins. If there are not enough resources to make the drink, the user is informed that the machine cannot fulfill the order. The profit variable is updated whenever a transaction is successful.

In summary, the code simulates a coffee machine that can receive orders, calculate payments, and deduct resources.
