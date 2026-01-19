# Sport-obud-shop.mn
<!obud shop html>
<html lang="mn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sport Obud Shop</title>

<style>
body {
  margin: 0;
  padding: 15px;
  background: #0e0e0e;
  color: #fff;
  font-family: Arial, sans-serif;
}

h1 {
  text-align: center;
  margin-bottom: 15px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 12px;
}

.card {
  background: #1c1c1c;
  border-radius: 12px;
  padding: 10px;
  text-align: center;
}

.card img {
  width: 100%;
  height: 140px;
  object-fit: cover;
  border-radius: 10px;
}

.name {
  margin: 8px 0 4px;
  font-size: 14px;
  font-weight: bold;
}

.price {
  color: #00ff99;
  font-weight: bold;
  margin-bottom: 8px;
}

button {
  background: #ff2e2e;
  border: none;
  border-radius: 20px;
  padding: 8px 14px;
  color: #fff;
  font-size: 14px;
  cursor: pointer;
}

button:active {
  transform: scale(0.95);
}
</style>
</head>

<body>

<h1>🔥 Sport Машины Обуд</h1>

<div class="grid" id="grid"></div>

<script>
const obud = [
  "BBS RS Sport","BBS LM Racing","RAYS Volk TE37","RAYS Gram Lights 57DR",
  "OZ Racing Ultraleggera","OZ Racing Superturismo","Enkei RPF1","Enkei NT03+M",
  "Work Emotion CR Kai","Work Meister S1","SSR GTX01","SSR Professor MS3",
  "HRE FlowForm FF10","HRE Performance P101","Rotiform BLQ","Rotiform RSE",
  "ADVAN Racing GT","ADVAN RG-D2","Konig Hypergram","Konig Dekagram"
];

const grid = document.getElementById("grid");

obud.forEach((name, i) => {
  grid.innerHTML += `
    <div class="card">
      <img src="https://source.unsplash.com/400x300/?car,rim,wheel&sig=${i}">
      <div class="name">${name}</div>
      <div class="price">1,000₮</div>
      <button onclick="troll()">Авах</button>
    </div>
  `;
});

function troll() {
  alert("🚗💨 Май сда\nОбуд байхгүй, мөрөөдөөд л яв 🤣");
}
</script>

</body>
</html>
