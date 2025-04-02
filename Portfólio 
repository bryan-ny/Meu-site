<!DOCTYPE html>
<html lang="pt-br">
<head> 
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Portfólio</title>
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
            padding: 20px;
            text-align: center;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            justify-content: center;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            text-decoration: none;
            color: white;
            font-size: 18px;
        }

        section {
            padding: 40px;
            text-align: center;
        }

        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .project-card {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
        }
    </style>
  

</head>

<body>
 
        <h1>Meu Portfólio</h1>
        <nav>
            <ul>
                
                <li><a href="#projetos">Projetos</a></li>
                <li><a href="#sobre">Sobre Mim</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <section id="projetos">
        <h2>Meus Projetos</h2>
        <div class="projects">
            <div class="project-card">
                <h3>Projeto 1</h3>
                <p>Descrição do projeto 1.
                  <br>                  
                   É um projeto de coversão de moeda
                  <br>
                  (Dolar, Euro, Real)
                </p>
              <header>
        <h1>Simulador de Cotação de Moeda</h1>
    </header>

    <div class="container">
        <div class="calculator">
            <h2>Converter Moeda</h2>
            <input type="number" id="valor" placeholder="Valor" />
            <select id="moeda-origem">
                <option value="USD">Dólar (USD)</option>
              
                <option value="EUR">Euro (EUR)</option>
                <option value="BRL">Real (BRL)</option>
            </select>
            <span>para</span>
            <select id="moeda-destino">
                <option value="USD">Dólar (USD)</option> 
                <option value="EUR">Euro (EUR)</option>
                <option value="BRL">Real (BRL)</option>
            </select>
            <button onclick="converter()">Converter</button>
            <h3 id="resultado"></h3>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 Simulador de Cotação de Moeda</p>
    </footer>

    <script>
        // Cotações simuladas
        const cotacoes = {
            'USD': .1,
            'EUR': 0.92,
            'BRL': 5.45
        };

        function converter() {
            const valor = parseFloat(document.getElementById('valor').value);
            const moedaOrigem = document.getElementById('moeda-origem').value;
            const moedaDestino = document.getElementById('moeda-destino').value;

            if (!valor || valor <= 0) {
                alert('Por favor, insira um valor válido.');
                return;
            }

            const valorConvertido = (valor * cotacoes[moedaDestino] / cotacoes[moedaOrigem]).toFixed(2);
            document.getElementById('resultado').textContent = `${valor} ${moedaOrigem} = ${valorConvertido} ${moedaDestino}`;
        }
    </script>
              
              
            </div>
            <div class="project-card">
                <h3>Projeto 2</h3>

           <p>
             <em> Descrição do projeto 2.</em>
             <br>
               É um relogio que funciona em tempo real
             <br>
             (Horario de Brasilia)
           </p>
              <header><h1>Relogio em Tempo Real</h1></header>
              <br>
              <br>
              
          <div class="clock">
        <div id="digital-clock"></div>
        <div class="analog-clock">
            <div class="hour" id="hour-hand"></div>
            <div class="minute" id="minute-hand"></div>
            <div class="second" id="second-hand"></div>
        </div>
    </div>

    <script>
        function updateClock() {
            const now = new Date();
            const hours = now.getHours();
            const minutes = now.getMinutes();
            const seconds = now.getSeconds();

            // Digital Clock
            const digitalClock = document.getElementById('digital-clock');
            digitalClock.textContent = `${hours.toString().padStart(2, '0')}:${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;

            // Analog Clock
            const hourHand = document.getElementById('hour-hand');
            const minuteHand = document.getElementById('minute-hand');
            const secondHand = document.getElementById('second-hand');

            const hourDegree = (hours % 12) * 30 + (minutes / 2); // 360° / 12 hours
            const minuteDegree = minutes * 6; // 360° / 60 minutes
            const secondDegree = seconds * 6; // 360° / 60 seconds

            hourHand.style.transform = `rotate(${hourDegree}deg)`;
            minuteHand.style.transform = `rotate(${minuteDegree}deg)`;
            secondHand.style.transform = `rotate(${secondDegree}deg)`;
        }

        setInterval(updateClock, 1000);
        updateClock(); // Initial call to display clock immediately
    </script>
    
            </div>
            <div class="project-card">
                <h3>Projeto 3</h3>
                <p>Descrição do projeto 3.
                  <br>
                  É projeto de um Mercado online Simples
                  <br>
                  (prototipo)
                </a></p> 
         
              <div class="container">
                <header> <h1>E-commerce Simples</h1></header>
        <div class="products" id="product-list"></div>

        <div class="cart">
            <h2>Carrinho</h2>
            <ul id="cart-list"></ul>
            <p>Total: R$<span id="total">0.00</span></p>
        </div>
    </div>

    <script>
        const products = [
            { id: 1, name: 'Produto 1', price: 26.50 },
            { id: 2, name: 'Produto 2', price: 48.35},
            { id: 3, name: 'Produto 3', price: 19.70 },
            { id: 4, name: 'Produto 4', price: 93.99 }
        ];

        let cart = [];

        const productList = document.getElementById('product-list');
        const cartList = document.getElementById('cart-list');
        const totalElement = document.getElementById('total');

        function renderProducts() {
            productList.innerHTML = products.map(product => `
                <div class="product">
                    <h3>${product.name}</h3>
                    <p>R$${product.price.toFixed(2)}</p>
                    <button onclick="addToCart(${product.id})">Adicionar ao Carrinho</button>
                </div>
            `).join('');
        }

        function addToCart(id) {
            const product = products.find(prod => prod.id === id);
            cart.push(product);
            renderCart();
        }

        function renderCart() {
            cartList.innerHTML = cart.map((item, index) => `
                <li>${item.name} - R$${item.price.toFixed(2)} <button onclick="removeFromCart(${index})">Remover</button></li>
            `).join('');

            const total = cart.reduce((sum, item) => sum + item.price, 0);
            totalElement.textContent = total.toFixed(2);
        }

        function removeFromCart(index) {
            cart.splice(index, 1);
            renderCart();
        }

        renderProducts();
    </script>
            </div>
          
        </div>
    </section>

    <section id="sobre">
        <h2>Sobre Mim</h2>
        <p>Olá! Sou um desenvolvedor novato,entusiasmado para criar sites e aplicações modernas, responsivas e legais.</p>
    </section>

    <section id="contato">
        <h2>Contato</h2>
        <p>Envie uma Mensagem para: (41) 999423803
            <br>
        ou entre em contato cilcando no batão abaixo </p>
 <h1>↯</h1>
            

<a href="https://www.instagram.com/_bryann.andre" target="_blank" style="text-decoration: none;">
    <button style="display: flex; align-items: center; background-color: #E1306C; color: white; border: none; padding: 10px 20px; font-size: 16px; border-radius: 5px; cursor: pointer;">
        <img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" width="20" height="20" style="margin-right: 10px;">
        Meu Instagram
    </button>
</a>


    </section>

    <footer>
        <p>&copy; 2025 Meu Portfólio. Todos os direitos reservados.</p>
    </footer>


  
</body>
</html>