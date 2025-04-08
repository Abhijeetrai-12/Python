# Python
Restaurant management System using python (Mini project)
<---------Here's is a Code.------------------->
# Define the menu of a restaurant
Menu = {
    'Pizza':40,
    'Pasta':50,
    'Burger':60,
    'salad':70,
    'coffee':80,
    'maggie':35,
    'chai':10,
}
print(Menu)
#Greet
print("welcome to ABHIJEET's RESTAURANT")
print("Pizza:Rs40\nPasta:Rs50\nBurger:Rs60\nSalad:Rs70\nCoffee:Rs80\nMaggie:Rs35\nChai:Rs10")
Order_total = 0 
item_1 = input("Enter the name of item you want to order=")
if item_1 in Menu :
    Order_total+=Menu[item_1]
    print(f"your item {item_1} has been added to your order")
else:
    
    another_order=input("Do you want to add another item ? (Yes/No)")
    if another_order== "Yes":
        item_2 = input("enter the name of second item=")
        if item_2 in Menu:
            Order_total+=Menu[item_2]
            print(f"item {item_2} has been added to order")
        else:
            print(f"ordered item {item_2} is not available!")
            print(f" The total amount of items to pay is {Order_total}")    
