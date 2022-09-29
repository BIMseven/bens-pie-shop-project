# Ben's Pie Shop
Welcome to Ben's Pie Shop! I have cripling social anxiety and need to keep my business afloat. I cater only to customers with a strong understanding of java, or a love of the movie War Games. As such I need a command line interface (CLI) to greet fellow lovers of pie and take their money.

Your mission, should you choose to accept it, is to write said CLI.

## Functional Requirements
- Users are greeted with a message welcoming them to Ben's Pie Shop upon launching the program.
- Users interact with the system using the command line
- Users are asked if they want an appetizer/pizza/pie before menu options are displayed. They may respond with y for yes, n for no.
- If a user selects n when prompted for a type of menu item, the program continues to the next ordering phase.
- Users are prompted to select an appetizer (something pie themed... maybe a mini ciche)
- Users are prompted to select a type of Pizza (any option you can think of, with at least one anchovie option)
- Users are prompted to select a dessert pie (Pecan is my favorite)
- Each menu item when presented has an associated price
- Menu items printed at each step are selectable by entering 0.. number of options
- After the order is taken the total price is printed
- (Bonus) Give the user an option to add a suggested tip, one of 15% , 20%, 69% of the original total order
- The pie shop system you design should be scalable, meaning that I want it to be easy for me to add new menu items
- (Bonus) The pie shop is testable... write unit tests!

## Technical Requirements
- Most of your business logic should be placed in a java class called PieShop.java
- You may choose any library for printing to the console and reading user input from the console
- Menu items should be defined using an enum.
- You are encourage to use the cli command javac to compile your code and java <name of the class that contains your main(String[] args) method to run your code.
- unrecognized user responses simply print out the previous message again (and does not crash the program)


## Example console output
```log
Welcome to Ben's Pie Shop, home of the famous Pie in the Sky!
Would you like any appetizers (y/n)?
> y
We have [0] Classic Quiche ($4.00), [1] Bacon Quiche ($5.00)
> 0
Would you like a Pizza (y/n)?
> y
We have [0] Plain ($8.00), [1] Pepperoni ($9.00), [2] Anchovie ($9.50)
> 2
Would you like a Pie for dessert (y/n)?
> n
Your total is: $13.50, would you like to add a tip (y/n)?
> n
Okay your grand total is: $13.50, enjoy your meal (cheapskate) // note, calling the customer names if they don't tip is optional
```

