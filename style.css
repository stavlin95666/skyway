function addToCart(name, price) {
  const cart = JSON.parse(localStorage.getItem("cart")) || [];
  cart.push({ name, price });
  localStorage.setItem("cart", JSON.stringify(cart));
  alert(${name} added to cart!);
}

if (document.getElementById("cart-items")) {
  const cart = JSON.parse(localStorage.getItem("cart")) || [];
  const cartItems = document.getElementById("cart-items");
  const totalDiv = document.getElementById("total-price");
  if (cart.length === 0) {
    cartItems.innerHTML = "<p>Cart is empty</p>";
  } else {
    let total = 0;
    cart.forEach(item => {
      total += item.price;
      const p = document.createElement("p");
      p.textContent = ${item.name} – ₹${item.price};
      cartItems.appendChild(p);
    });
    totalDiv.textContent = Total: ₹${total};
  }
}
