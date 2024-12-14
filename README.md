# crochetopia.github.io
er {
    background-color: #ff6fb5;
    color: white;
  }
  
  .categories, .products, .cart {
    padding: 20px;
  }
  
  .category-list {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
    justify-content: center;
  }
  
  .category-item {
    background-color: #ffe3ee;
    padding: 20px;
    border-radius: 15px;
    text-align: center;
    cursor: pointer;
    border: 1px solid #ffaad4;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s, box-shadow 0.3s;
  }
  
  .category-item:hover {
    transform: scale(1.1);
    box-shadow: 0 6px 10px rgba(0, 0, 0, 0.2);
  }
  
  .product-list {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
  }
  
  .product-item {
    border: 1px solid #ffd1e5;
    padding: 15px;
    width: 220px;
    text-align: center;
    border-radius: 15px;
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s, box-shadow 0.3s;
  }
  
  .product-item img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    margin-bottom: 10px;
  }
  
  .product-item:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
  }
  
  .cart-list {
    margin-top: 10px;
  }
  
  .cart-total {
    margin-top: 15px;
    font-size: 18px;
    font-weight: bold;
  }
  
  button {
    cursor: pointer;
    padding: 10px 15px;
    border-radius: 25px;
    background-color: #ff6fb5;
    color: white;
    border: none;
    transition: all 0.3s;
  }
  
  button:hover {
    background-color: #ff4081;
  }
  
  .modal {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgba(0, 0, 0, 0.5);
    justify-content: center;
    align-items: center;
    animation: fadeIn 0.3s;
  }
  
  .modal-content {
    background-color: white;
    padding: 30px;
    border-radius: 15px;
    text-align: center;
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
  }
  
  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }
  
  /* Cute placeholder images */
  
  
  .category-item::before {
    content: '💖';
    margin-right: 8px;
  }  
.cart {
    padding: 30px;
    background: linear-gradient(135deg, #ffd1e5, #ffeaf4);
    border-radius: 15px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
    max-width: 600px;
    margin: 20px auto;
    animation: popCart 0.3s ease-in-out;
    position: relative;
  }
  
  .cart h2 {
    font-size: 24px;
    font-weight: bold;
    color: #ff4081;
    text-align: center;
    margin-bottom: 20px;
  }
  
  .cart-list {
    background-color: #fff;
    padding: 15px;
    border-radius: 10px;
    box-shadow: inset 0 2px 6px rgba(0, 0, 0, 0.1);
    max-height: 200px;
    overflow-y: auto;
  }
  
  .cart-item {
    display: flex;
    justify-content: space-between;
    padding: 10px 0;
    border-bottom: 1px dashed #ffd1e5;
    font-size: 16px;
  }
  
  .cart-item:last-child {
    border-bottom: none;
  }
  
  .cart-total {
    margin-top: 20px;
    font-size: 22px;
    font-weight: bold;
    text-align: center;
    color: #d243cb;
    background: #ffeaf4;
    padding: 10px;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  }
  
  .cart-total span {
    color: #ff4081;
  }
  
  #checkout-link {
    display: block;
    text-align: center;
    margin-top: 20px;
    text-decoration: none;
  }
  
  #checkout-link button {
    background: linear-gradient(135deg, #ffaad4, #ff6fb5);
    color: white;
    font-size: 16px;
    padding: 10px 20px;
    border-radius: 25px;
    border: none;
    transition: all 0.3s;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  }
  
  #checkout-link button:hover {
    background: linear-gradient(135deg, #ff4081, #ff6fb5);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
    transform: translateY(-2px);
  }
  
  @keyframes popCart {
    0% {
      transform: scale(0.95);
      opacity: 0;
    }
    100% {
      transform: scale(1);
      opacity: 1;
    }
  }
  /* Updated Checkout Button */
#checkout-link button {
    background: linear-gradient(135deg, #ffaad4, #ff6fb5);
    color: white;
    font-size: 18px;
    font-weight: bold;
    padding: 12px 25px;
    border-radius: 30px;
    border: none;
    transition: all 0.3s ease-in-out;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
  }
  
  #checkout-link button::after {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 300%;
    height: 100%;
    background: rgba(255, 255, 255, 0.3);
    transform: skewX(-45deg);
    transition: all 0.5s;
  }
  
  #checkout-link button:hover {
    background: linear-gradient(135deg, #ff6fb5, #ff4081);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
  }
  
  #checkout-link button:hover::after {
    left: 100%;
  }
  
  /* Unique Emojis for Categories */
  .category-list .category-item:nth-child(1)::before {
    content: '🌹'; /* Example: Accessories */
  }
  
  .category-list .category-item:nth-child(2)::before {
    content: '👗'; /* Example: Dresses */
  }
  
  .category-list .category-item:nth-child(3)::before {
    content: '🧥'; /* Example: Shoes */
  }
  
  .category-list .category-item:nth-child(4)::before {
    content: '🧸'; /* Example: Hair Accessories */
  }
  
  .category-list .category-item:nth-child(5)::before {
    content: '👝'; /* Example: Makeup */
  }
  
  .category-list .category-item {
    position: relative;
    font-weight: bold;
  }
  
  .category-item::before {
    margin-right: 10px;
    font-size: 20px;
  }
  

const products = [
    { id: 1, name: "Flowers", price: 150, image: "flower.jpg" },
    { id: 2, name: "Tops", price: 799, image: "top.jpg" },
    { id: 3, name: "Sweaters", price: 1300, image: "sweater.jpg" },
    { id: 4, name: "Toys", price: 400, image: "toy.jpg" },
    { id: 5, name: "Pouches", price: 600, image: "pouch.jpg" },
    { id: 6, name: "Accessories", price: 350, image: "accessory.jpg" },
  ];
  
  const productList = document.getElementById("product-list");
  const cartList = document.getElementById("cart-list");
  const totalCostElement = document.getElementById("total-cost");
  const checkoutModal = document.getElementById("checkout-modal");
  let cart = [];
  let totalCost = 0;
  
  // Render products
  function renderProducts(productsToRender) {
    productList.innerHTML = "";
    productsToRender.forEach((product) => {
      const productElement = document.createElement("div");
      productElement.className = "product-item";
      productElement.innerHTML = `
        <img src="${product.image}" alt="${product.name}" class="product-image" />
        <h3>${product.name}</h3>
        <p>${product.price} Rupees</p>
        <button onclick="addToCart(${product.id})">Add to Cart</button>
      `;
      productList.appendChild(productElement);
    });
  }
  
  // Add to cart
  function addToCart(productId) {
    const product = products.find((item) => item.id === productId);
    cart.push(product);
    const cartItem = document.createElement("div");
    cartItem.textContent = `${product.name} - ${product.price} Rupees`;
    cartList.appendChild(cartItem);
    totalCost += product.price;
    totalCostElement.textContent = totalCost;
  }
  
  // Search functionality
  document.getElementById("search-btn").addEventListener("click", () => {
    const query = document.getElementById("search-input").value.toLowerCase();
    const filteredProducts = products.filter((product) =>
      product.name.toLowerCase().includes(query)
    );
    renderProducts(filteredProducts);
  });
  
  // Show checkout modal
  document.getElementById("checkout-btn").addEventListener("click", () => {
    checkoutModal.style.display = "flex";
  });
  
  // Place order
  document.getElementById("checkout-form").addEventListener("submit", (e) => {
    e.preventDefault();
    const address = document.getElementById("address").value;
    alert(`Order placed! Address: ${address}\nPayment: Cash on Delivery`);
    cart = [];
    cartList.innerHTML = "";
    totalCost = 0;
    totalCostElement.textContent = totalCost;
    checkoutModal.style.display = "none";
  });
  
  // Initial render
  renderProducts(products);


<?php
header('Content-Type: application/json');
$servername = "localhost";
$username = "root";  // Replace with your DB username
$password = "";      // Replace with your DB password
$dbname = "crochetopia";

$conn = new mysqli($servername, $username, $password, $dbname);

if ($conn->connect_error) {
    die(json_encode(["error" => "Connection failed: " . $conn->connect_error]));
}

$action = $_GET['action'] ?? '';

if ($action === 'getProducts') {
    $sql = "SELECT * FROM products";
    $result = $conn->query($sql);
    $products = [];
    while ($row = $result->fetch_assoc()) {
        $products[] = $row;
    }
    echo json_encode($products);
} elseif ($action === 'placeOrder') {
    $data = json_decode(file_get_contents('php://input'), true);
    $address = $data['address'];
    $cart = $data['cart'];
    $totalCost = $data['totalCost'];

    $conn->begin_transaction();
    try {
        $sql = "INSERT INTO orders (address, total_cost) VALUES (?, ?)";
        $stmt = $conn->prepare($sql);
        $stmt->bind_param("sd", $address, $totalCost);
        $stmt->execute();
        $orderId = $stmt->insert_id;

        foreach ($cart as $item) {
            $sql = "INSERT INTO order_items (order_id, product_id, quantity) VALUES (?, ?, ?)";
            $stmt = $conn->prepare($sql);
            $stmt->bind_param("iii", $orderId, $item['id'], $item['quantity']);
            $stmt->execute();
        }
        $conn->commit();
        echo json_encode(["success" => true, "orderId" => $orderId]);
    } catch (Exception $e) {
        $conn->rollback();
        echo json_encode(["error" => "Order placement failed."]);
    }
}

$conn->close();
?>



