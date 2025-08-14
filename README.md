# week 3 assignment
def calculate_discount(price, discount_percentage):
   
   if discount_percentage>=20:
         discount = price * (discount_percentage / 100)
         final_price = price - discount
         return final_price
   else:
         return price
   
try:
        price = float(input("Enter the price of the item: "))
        discount_percentage = float(input("Enter the discount percentage: "))
        
        final_price = calculate_discount(price, discount_percentage)
        print(f"The final price after discount is: {final_price}")
except ValueError:
        print("Invalid input. Please enter numeric values for price and discount percentage.")
