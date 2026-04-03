<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>O'Bay Market</title>

<style>
body {
    font-family: Arial;
    margin: 0;
    background: #f5f5f5;
}

header {
    background: #2c3e50;
    color: white;
    padding: 15px;
    text-align: center;
}

.container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 20px;
}

.card {
    background: white;
    width: 200px;
    margin: 10px;
    padding: 15px;
    border-radius: 10px;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}

.card img {
    width: 100%;
    border-radius: 10px;
}

button {
    margin-top: 10px;
    padding: 10px;
    border: none;
    background: green;
    color: white;
    cursor: pointer;
    border-radius: 5px;
}

.cart {
    position: fixed;
    top: 10px;
    right: 10px;
    background: orange;
    padding: 10px;
    border-radius: 10px;
    color: white;
}
</style>
</head>

<body>

<header>
    <h1>Toko Online Saya</h1>
</header>

<div class="cart">
    🛒 Keranjang: <span id="total">0</span>
</div>

<div class="container">

    <div class="card">
        <img src="https://via.placeholder.com/200">
        <h3>T-shirt</h3>
        <p>Rp 50.000</p>
        <button onclick="beli()">Beli</button>
    </div>

    <div class="card">
        <img src="https://via.placeholder.com/200">
        <h3>Shoes</h3>
        <p>Rp 75.000</p>
        <button onclick="beli()">Beli</button>
    </div>

    <div class="card">
        <img src="https://via.placeholder.com/200">
        <h3>Pants</h3>
        <p>Rp 100.000</p>
        <button onclick="beli()">Beli</button>
    </div>

</div>

<script>
let total = 0;

function beli() {
    total++;
    document.getElementById("total").innerText = total;
    alert("Produk ditambahkan ke keranjang!");
}
</script>

</body>
</html>
