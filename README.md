<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Online Shop</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f0f0f0;
    }
    header {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 20px;
    }
    #cart {
      position: fixed;
      top: 20px;
      right: 20px;
      background-color: #ff9800;
      padding: 10px 15px;
      border-radius: 5px;
      font-weight: bold;
    }
    .container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 20px;
    }
    .product {
      background-color: white;
      border-radius: 8px;
      margin: 10px;
      padding: 15px;
      width: 220px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .product img {
      max-width: 100%;
      border-radius: 5px;
    }
    .product h3 {
      margin: 10px 0 5px;
    }
    .product p {
      margin: 5px 0;
      font-weight: bold;
    }
    .product button {
      background-color: #28a745;
      color: white;
      border: none;
      padding: 10px;
      margin-top: 10px;
      border-radius: 5px;
      cursor: pointer;
    }
    .product button:hover {
      background-color: #218838;
    }
  </style>
</head>
<body>

<header>
  <h1>My Online Shop</h1>
</header>

<div id="cart">Cart: 0 items</div>

<div class="container">
  <div class="product">
    <img src="https://via.placeholder.com/150" alt="Product 1">
    <h3>Product 1</h3>
    <p>$10.00</p>
    <button onclick="addToCart()">Add to Cart</button>
  </div>
  <div class="product">
    <img src="https://via.placeholder.com/150" alt="Product 2">
    <h3>Product 2</h3>
    <p>$15.00</p>
    <button onclick="addToCart()">Add to Cart</button>
  </div>
  <div class="product">
    <img src="https://via.placeholder.com/150" alt="Product 3">
    <h3>Product 3</h3>
    <p>$20.00</p>
    <button onclick="addToCart()">Add to Cart</button>
  </div>
</div>

<script>
  let cartCount = 0;
  function addToCart() {
    cartCount++;
    document.getElementById('cart').textContent = `Cart: ${cartCount} items`;
  }
</script>

</body>
</html>
