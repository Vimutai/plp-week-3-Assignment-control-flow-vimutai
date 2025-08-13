📉 Discount Calculator
A Python function that calculates the final price after applying a discount (if eligible).

📌 Features
✅ Calculates discounted price if discount is 20% or higher.
✅ Returns the original price if the discount is too low.
✅ Simple user input/output interaction.

🚀 How to Use
Clone the repository:

bash
[git clone https://github.com/Vimutai/plp-week-3-Assignment-control-flow-vimutai.git]
cd discount-calculator
Run the script:

bash
python discount_calculator.py
Enter the required inputs:

Original price (e.g., 100)

Discount percentage (e.g., 25)

Get the result:

If discount ≥ 20%, it applies the discount.

Otherwise, it returns the original price.

Example Output
text
Enter the original price of the item: 100  
Enter the discount percentage: 25  
Final price after 25% discount: $75.00  
🛠️ Code Structure
python
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        return price * (1 - discount_percent / 100)
    else:
        return price

# User input & output logic
original_price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))
final_price = calculate_discount(original_price, discount_percent)

if discount_percent >= 20:
    print(f"Final price after {discount_percent}% discount: ${final_price:.2f}")
else:
    print(f"No discount applied. Original price: ${original_price:.2f}")
📜 License
This project is open-source under the MIT License.

📌 How to Add README.md to Your Repo
Create a new file named README.md in your repo.

Paste the content above.

Commit and push:

bash
git add README.md
git commit -m "Added README documentation"
git push origin main