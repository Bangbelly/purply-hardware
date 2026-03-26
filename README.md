<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Purply Hardware</title>

<style>
body { margin:0; font-family:Segoe UI, sans-serif; background:#f4f4f8; transition:0.3s; }
.dark { background:#121212; color:#eee; }
header { background:linear-gradient(135deg,#4b006e,#7b1fa2); color:white; padding:25px; text-align:center; }
nav { display:flex; justify-content:center; gap:25px; background:#111; padding:15px; }
nav a { color:white; text-decoration:none; font-weight:bold; cursor:pointer; }
nav a:hover { color:#c77dff; }
section { display:none; padding:40px 20px; max-width:1100px; margin:auto; }
.active { display:block; }
.card { background:white; padding:25px; border-radius:15px; box-shadow:0 5px 15px rgba(0,0,0,0.1); margin-bottom:20px; }
.dark .card { background:#1e1e1e; }
.hero { height:300px; background:url('https://images.unsplash.com/photo-1503387762-592deb58ef4e') center/cover; display:flex; align-items:center; justify-content:center; color:white; font-size:30px; font-weight:bold; border-radius:15px; }
.gallery { display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:20px; }
.product { background:white; border-radius:12px; padding:10px; text-align:center; box-shadow:0 3px 10px rgba(0,0,0,0.1); }
.dark .product { background:#1e1e1e; }
.product img { width:100%; height:180px; object-fit:cover; border-radius:10px; }
.price { color:#7b1fa2; font-weight:bold; }
button { margin-top:8px; padding:8px 12px; border:none; background:#7b1fa2; color:white; border-radius:8px; cursor:pointer; }
footer { background:#111; color:white; text-align:center; padding:20px; }
.whatsapp { position:fixed; bottom:20px; right:20px; background:#25D366; color:white; padding:15px 18px; border-radius:50px; text-decoration:none; font-weight:bold; }
.toggle { position:fixed; top:20px; right:20px; background:#000; color:white; padding:8px 12px; border-radius:20px; cursor:pointer; }
.logo { font-size:22px; font-weight:bold; }
</style>

<script>
function showPage(pageId) {
  document.querySelectorAll('section').forEach(sec => sec.classList.remove('active'));
  document.getElementById(pageId).classList.add('active');
}

function orderItem(item) {
  const url = `https://wa.me/254720200329?text=Hello Purply Hardware, I want to order ${item}`;
  window.open(url, '_blank');
}

function toggleDark() {
  document.body.classList.toggle('dark');
}
</script>

</head>
<body onload="showPage('home')">

<div class="toggle" onclick="toggleDark()">Dark Mode</div>

<header>
<div class="logo">🟣 Purply Hardware</div>
<p>Premium Construction Materials Supplier</p>
</header>

<nav>
<a onclick="showPage('home')">Home</a>
<a onclick="showPage('about')">About</a>
<a onclick="showPage('products')">Products</a>
<a onclick="showPage('contact')">Contact</a>
</nav>

<section id="home">
<div class="hero">Quality Materials. Trusted Service.</div>
<div class="card">
<h2>Welcome</h2>
<p>We provide strong, affordable and reliable construction materials in Jericho. Trusted by fundis and contractors for quality and fast service.</p>
</div>
</section>

<section id="about">
<div class="card">
<h2>About Us</h2>
<p>Purply Hardware supplies sand, cement, mabati (iron sheets), plywood and more. We focus on quality products and customer satisfaction.</p>
</div>
</section>

<section id="products">
<div class="card">
<h2>Products & Prices</h2>
<div class="gallery">

<div class="product">
<img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c">
<p>Sand</p>
<p class="price">KSh 250</p>
<button onclick="orderItem('Sand')">Order</button>
</div>

<div class="product">
<img src="https://images.unsplash.com/photo-1621905251918-48416bd8575a">
<p>Dust</p>
<p class="price">KSh 200</p>
<button onclick="orderItem('Dust')">Order</button>
</div>

<div class="product">
<img src="https://images.unsplash.com/photo-1590658268037-6bf12165a8df">
<p>Cement</p>
<p class="price">KSh 800</p>
<button onclick="orderItem('Cement')">Order</button>
</div>

<div class="product">
<img src="https://images.unsplash.com/photo-1581578731548-c64695cc6952">
<p>Plywood</p>
<p class="price">KSh 550</p>
<button onclick="orderItem('Plywood')">Order</button>
</div>

<div class="product">
<img src="https://images.unsplash.com/photo-1618220179428-22790b461013">
<p>Mabati Gauge 2</p>
<p class="price">KSh 700</p>
<button onclick="orderItem('Mabati Gauge 2')">Order</button>
</div>

<div class="product">
<img src="https://images.unsplash.com/photo-1618220179428-22790b461013">
<p>Mabati Gauge 2.5</p>
<p class="price">KSh 800</p>
<button onclick="orderItem('Mabati Gauge 2.5')">Order</button>
</div>

<div class="product">
<img src="https://images.unsplash.com/photo-1618220179428-22790b461013">
<p>Mabati Gauge 3</p>
<p class="price">KSh 900</p>
<button onclick="orderItem('Mabati Gauge 3')">Order</button>
</div>

<div class="product">
<img src="https://images.unsplash.com/photo-1581578017093-cd30fce4eeb7">
<p>Mops</p>
<p class="price">KSh 200</p>
<button onclick="orderItem('Mops')">Order</button>
</div>

<div class="product">
<img src="https://images.unsplash.com/photo-1562259949-e8e7689d7828">
<p>Paint (20L)</p>
<p class="price">KSh 3,500</p>
<button onclick="orderItem('Paint')">Order</button>
</div>

<div class="product">
<img src="https://images.unsplash.com/photo-1565610222536-ef125c59da2e">
<p>Steel Bars</p>
<p class="price">KSh 800 - 1,500</p>
<button onclick="orderItem('Steel Bars')">Order</button>
</div>

</div>
</div>
</section>

<section id="contact">
<div class="card">
<h2>Contact</h2>
<p>0720200329 / 0723880918</p>
<p>Jericho</p>
</div>
</section>

<footer>
<p>&copy; 2026 Purply Hardware</p>
</footer>

<a class="whatsapp" href="https://wa.me/254720200329" target="_blank">Chat on WhatsApp</a>

</body>
</html>
