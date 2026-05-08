
const products = [
  {
    name: "壓克力立牌",
    krw: 12000,
    twd: 285,
    image: "https://picsum.photos/400?1",
    qty: 0
  },
  {
    name: "拍立得",
    krw: 8000,
    twd: 190,
    image: "https://picsum.photos/400?2",
    qty: 0
  },
  {
    name: "特裝版",
    krw: 45000,
    twd: 1080,
    image: "https://picsum.photos/400?3",
    qty: 0
  }
];

const productList = document.getElementById("product-list");

function renderProducts() {
  productList.innerHTML = "";

  products.forEach((product, index) => {
    const div = document.createElement("div");
    div.className = "product";

    div.innerHTML = `
      <img src="${product.image}">
      <h3>${product.name}</h3>
      <div class="price">
        ₩${product.krw.toLocaleString()}<br>
        NT$${product.twd.toLocaleString()}
      </div>

      <div class="qty-box">
        <button onclick="changeQty(${index}, -1)">-</button>
        <span>${product.qty}</span>
        <button onclick="changeQty(${index}, 1)">+</button>
      </div>
    `;

    productList.appendChild(div);
  });

  updateTotals();
}

function changeQty(index, amount) {
  products[index].qty += amount;

  if (products[index].qty < 0) {
    products[index].qty = 0;
  }

  renderProducts();
}

function updateTotals() {
  let krw = 0;
  let twd = 0;

  products.forEach(product => {
    krw += product.krw * product.qty;
    twd += product.twd * product.qty;
  });

  document.getElementById("krwTotal").innerText =
    `₩${krw.toLocaleString()}`;

  document.getElementById("twdTotal").innerText =
    `NT$${twd.toLocaleString()}`;

  document.getElementById("codTotal").innerText =
    `NT$${twd.toLocaleString()}`;

  updateRemain();
}

function updateRemain() {
  let twd = 0;

  products.forEach(product => {
    twd += product.twd * product.qty;
  });

  const bankAmount =
    Number(document.getElementById("bankAmount")?.value || 0);

  const nocardAmount =
    Number(document.getElementById("nocardAmount")?.value || 0);

  document.getElementById("bankRemain").innerText =
    `NT$${(twd - bankAmount).toLocaleString()}`;

  document.getElementById("nocardRemain").innerText =
    `NT$${(twd - nocardAmount).toLocaleString()}`;
}

document.querySelectorAll('input[name="payment"]').forEach(radio => {
  radio.addEventListener("change", (e) => {
    document.getElementById("bank-section").classList.add("hidden");
    document.getElementById("nocard-section").classList.add("hidden");
    document.getElementById("cod-section").classList.add("hidden");

    if (e.target.value === "bank") {
      document.getElementById("bank-section").classList.remove("hidden");
    }

    if (e.target.value === "nocard") {
      document.getElementById("nocard-section").classList.remove("hidden");
    }

    if (e.target.value === "cod") {
      document.getElementById("cod-section").classList.remove("hidden");
    }
  });
});

document.getElementById("bankAmount")
  .addEventListener("input", updateRemain);

document.getElementById("nocardAmount")
  .addEventListener("input", updateRemain);

renderProducts();
