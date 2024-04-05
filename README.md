# Creative Shopping Web Application

## Description
This is a simple web application for an online shopping platform called "Creative Shopping". The application allows users to browse products, select quantities, and calculate the total price. It features a navigation bar, product listings with images, descriptions, and pricing. Users can update the quantity of each product, and the application dynamically calculates the total price, gross total, tax, and final payable amount.

## Technologies Used
- HTML
- CSS (Bootstrap 5.3.3)
- JavaScript

## Features
- Navigation bar with links to categories, bestsellers, and about page.
- Product listings with images, descriptions, and pricing.
- Quantity selection for each product.
- Dynamic calculation of total price, gross total, tax, and total payable amount.
- Responsive design.

## Screenshots
![image](https://github.com/vishaljha1710/cart-page/assets/77543816/48eed511-73f7-4a07-ae8a-4b30da3ea4b1)

![image](https://github.com/vishaljha1710/cart-page/assets/77543816/214a2c12-1408-4a00-b7bc-ff4f80f08edc)



## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/creative-shopping-web-app.git
    ```
2. Open `index.html` in a web browser.

## Usage
1. Navigate to the Creative Shopping web application.
2. Browse the available products.
3. Select the quantity of each product.
4. The application will dynamically calculate the total price, gross total, tax, and final payable amount.

## Code Snippets
### JavaScript Quantity Change Event
```javascript
const dropdown = document.getElementById("numberDropdown");
const dropdowncreatine = document.getElementById("numberDropdowncreatine");

dropdown.addEventListener("change", function() {
    const quantity = dropdown.value;
    const totalPrice = quantity * 4200;
    document.getElementById("total").textContent = totalPrice.toFixed(2);
    document.getElementById("grosstotalwhey").textContent = totalPrice.toFixed(2);

    const totalPriceWhey = parseFloat(document.getElementById("total").innerHTML);
    const totalPriceCreatine = parseFloat(document.getElementById("totalcreatine").innerHTML);
    const grossTotal = totalPriceWhey + totalPriceCreatine;
    document.getElementById("grosstotal").textContent = grossTotal.toFixed(2);

    const tax = grossTotal * 0.18;
    document.getElementById("tax").textContent = tax.toFixed(2);

    const totalpay = grossTotal + tax;
    document.getElementById("totalpay").textContent = totalpay.toFixed(2);
});

dropdowncreatine.addEventListener("change", function() {
    const quantity = dropdowncreatine.value;
    const totalPrice = quantity * 1200;
    document.getElementById("totalcreatine").textContent = totalPrice.toFixed(2);
    document.getElementById("grosstotalcreatine").textContent = totalPrice.toFixed(2);

    const totalPriceWhey = parseFloat(document.getElementById("total").innerHTML);
    const totalPriceCreatine = parseFloat(document.getElementById("totalcreatine").innerHTML);
    const grossTotal = totalPriceWhey + totalPriceCreatine;
    document.getElementById("grosstotal").textContent = grossTotal.toFixed(2);

    const tax = grossTotal * 0.18;
    document.getElementById("tax").textContent = tax.toFixed(2);

    const totalpay = grossTotal + tax;
    document.getElementById("totalpay").textContent = totalpay.toFixed(2);
});
Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

License
MIT

Contact
Website: Creative Shopping
Email: romanvkj2001@gmail.com
