# Ana-Beatriz
portfolio-pokemon-ana-beatriz/
│
├── index.html
├── styles.css
├── script.js
└── images/
    └── (coloque imagens de Pokémon aqui)
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfólio Pokémon - Ana Beatriz</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1>Portfólio Pokémon de Ana Beatriz</h1>
    <p>Confira alguns dos meus Pokémon favoritos!</p>
  </header>

  <div class="pokemon-cards">
    <!-- Card do Pokémon 1 -->
    <div class="card">
      <img src="images/pikachu.png" alt="Pikachu">
      <h2>Pikachu</h2>
      <p>Tipo: Elétrico</p>
    </div>

    <!-- Card do Pokémon 2 -->
    <div class="card">
      <img src="images/bulbasaur.png" alt="Bulbasaur">
      <h2>Bulbasaur</h2>
      <p>Tipo: Planta/Venenoso</p>
    </div>

    <!-- Card do Pokémon 3 -->
    <div class="card">
      <img src="images/charizard.png" alt="Charizard">
      <h2>Charizard</h2>
      <p>Tipo: Fogo/Voador</p>
    </div>

    <!-- Card do Pokémon 4 -->
    <div class="card">
      <img src="images/squirtle.png" alt="Squirtle">
      <h2>Squirtle</h2>
      <p>Tipo: Água</p>
    </div>
  </div>

  <script src="script.js"></script>
</body>
</html>
/* Resetando margens e padding */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Configuração do corpo */
body {
  font-family: Arial, sans-serif;
  background-color: #f0f0f0;
  color: #333;
  text-align: center;
  padding: 20px;
}

header {
  margin-bottom: 40px;
}

h1 {
  font-size: 2em;
  margin-bottom: 10px;
}

.pokemon-cards {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}

.card {
  background-color: white;
  border: 1px solid #ddd;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  width: 200px;
  margin: 10px;
  padding: 15px;
  text-align: center;
}

.card img {
  width: 100px;
  height: 100px;
  object-fit: contain;
}

.card h2 {
  font-size: 1.2em;
  margin: 10px 0;
}

.card p {
  font-size: 1em;
  color: #555;
}
document.querySelectorAll('.card').forEach(card => {
  card.addEventListener('click', () => {
    const pokemonName = card.querySelector('h2').textContent;
    alert(`Você clicou no ${pokemonName}!`);
  });
});
