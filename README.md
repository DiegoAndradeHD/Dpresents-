
<!DOCTYPE html><html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dpresents - O Universo Geek é Aqui!</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f0f0f5;
    }
    header {
      background-color: #1c1c3c;
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      display: flex;
      justify-content: center;
      background-color: #29294d;
      padding: 10px;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }
    .banner {
      background-image: url('https://via.placeholder.com/1200x400?text=Dpresents+Promo');
      background-size: cover;
      background-position: center;
      height: 400px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      font-size: 2.5rem;
      font-weight: bold;
    }
    .produtos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .produto {
      background: white;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      text-align: center;
      padding: 15px;
    }
    .produto img {
      width: 100%;
      height: 250px;
      object-fit: cover;
    }
    .produto button {
      background-color: #1c1c3c;
      color: white;
      border: none;
      padding: 10px 20px;
      margin-top: 10px;
      border-radius: 5px;
      cursor: pointer;
    }
    footer {
      background-color: #1c1c3c;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 20px;
    }
    .carrinho {
      padding: 20px;
    }
    .checkout {
      padding: 20px;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body><header>
  <h1>Dpresents</h1>
  <p>O Universo Geek é Aqui!</p>
</header><nav>
  <a href="#home" onclick="mostrarSessao('home')">Home</a>
  <a href="#produtos" onclick="mostrarSessao('produtos')">Produtos</a>
  <a href="#carrinho" onclick="mostrarSessao('carrinho')">Carrinho</a>
  <a href="#checkout" onclick="mostrarSessao('checkout')">Finalizar Compra</a>
  <a href="#sobre" onclick="mostrarSessao('sobre')">Sobre Nós</a>
  <a href="#contato" onclick="mostrarSessao('contato')">Contato</a>
</nav><section id="home" class="banner">
  Promoções Imperdíveis!
</section><section id="produtos" class="produtos">
  <div class="produto">
    <img src="https://via.placeholder.com/300x300?text=Camiseta+Anime" alt="Camiseta Anime">
    <h2>Camiseta Anime</h2>
    <p>R$ 79,90</p>
    <button onclick="adicionarCarrinho('Camiseta Anime', 79.90)">Adicionar ao Carrinho</button>
  </div>  <div class="produto">
    <img src="https://via.placeholder.com/300x300?text=Caneca+Heroi" alt="Caneca Herói">
    <h2>Caneca Herói</h2>
    <p>R$ 39,90</p>
    <button onclick="adicionarCarrinho('Caneca Herói', 39.90)">Adicionar ao Carrinho</button>
  </div>  <div class="produto">
    <img src="https://via.placeholder.com/300x300?text=Action+Figure" alt="Action Figure">
    <h2>Action Figure</h2>
    <p>R$ 199,90</p>
    <button onclick="adicionarCarrinho('Action Figure', 199.90)">Adicionar ao Carrinho</button>
  </div>
</section><section id="carrinho" class="carrinho hidden">
  <h2>Seu Carrinho</h2>
  <ul id="lista-carrinho"></ul>
  <p id="total"></p>
</section><section id="checkout" class="checkout hidden">
  <h2>Finalizar Compra</h2>
  <p>Preencha seus dados para concluir a compra:</p>
  <form>
    <input type="text" placeholder="Nome completo" required><br><br>
    <input type="email" placeholder="Email" required><br><br>
    <input type="text" placeholder="Endereço" required><br><br>
    <button type="submit">Confirmar Compra</button>
  </form>
</section><section id="
