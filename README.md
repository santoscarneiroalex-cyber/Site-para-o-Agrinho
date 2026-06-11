<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Campo e Cidade</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Campo e Cidade</h1>
    <nav>
        <a href="campo.html">Campo</a>
        <a href="cidade.html">Cidade</a>
        <a href="comparacao.html">Comparação</a>
    </nav>
</header>

<main>
    <h2>Bem-vindo!</h2>
    <p>Este site apresenta as características do campo e da cidade, mostrando suas diferenças e importância para a sociedade.</p>

    <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?w=800"
         alt="Paisagem" class="imagem">
</main>

<footer>
    <p>Projeto Escolar - Campo e Cidade</p>
</footer>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Campo</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Vida no Campo</h1>
    <nav>
        <a href="index.html">Home</a>
        <a href="cidade.html">Cidade</a>
        <a href="comparacao.html">Comparação</a>
    </nav>
</header>

<main>
    <h2>Características do Campo</h2>

    <ul>
        <li>Contato com a natureza</li>
        <li>Menor poluição</li>
        <li>Produção agrícola e pecuária</li>
        <li>Vida mais tranquila</li>
    </ul>

    <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?w=800"
         alt="Campo" class="imagem">
</main>

<footer>
    <p>Campo e Cidade</p>
</footer>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Cidade</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Vida na Cidade</h1>
    <nav>
        <a href="index.html">Home</a>
        <a href="campo.html">Campo</a>
        <a href="comparacao.html">Comparação</a>
    </nav>
</header>

<main>
    <h2>Características da Cidade</h2>

    <ul>
        <li>Maior oferta de empregos</li>
        <li>Serviços de saúde e educação</li>
        <li>Transporte público</li>
        <li>Grande concentração populacional</li>
    </ul>

    <img src="https://images.unsplash.com/photo-1477959858617-67f85cf4f1df?w=800"
         alt="Cidade" class="imagem">
</main>

<footer>
    <p>Campo e Cidade</p>
</footer>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Comparação</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Comparação entre Campo e Cidade</h1>
    <nav>
        <a href="index.html">Home</a>
        <a href="campo.html">Campo</a>
        <a href="cidade.html">Cidade</a>
    </nav>
</header>

<main>
    <table>
        <tr>
            <th>Campo</th>
            <th>Cidade</th>
        </tr>
        <tr>
            <td>Mais natureza</td>
            <td>Mais construções</td>
        </tr>
        <tr>
            <td>Menos trânsito</td>
            <td>Mais trânsito</td>
        </tr>
        <tr>
            <td>Produção de alimentos</td>
            <td>Comércio e indústria</td>
        </tr>
        <tr>
            <td>Vida tranquila</td>
            <td>Vida agitada</td>
        </tr>
    </table>
</main>

<footer>
    <p>Campo e Cidade</p>
</footer>

</body>
</html>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#f4f4f4;
    color:#333;
}

header{
    background:#2e8b57;
    color:white;
    text-align:center;
    padding:20px;
}

nav{
    margin-top:10px;
}

nav a{
    color:white;
    text-decoration:none;
    margin:0 10px;
    font-weight:bold;
}

main{
    max-width:900px;
    margin:30px auto;
    padding:20px;
    background:white;
    border-radius:10px;
}

.imagem{
    width:100%;
    margin-top:20px;
    border-radius:10px;
}

table{
    width:100%;
    border-collapse:collapse;
}

th{
    background:#2e8b57;
    color:white;
}

th, td{
    border:1px solid #ccc;
    padding:12px;
    text-align:center;
}

footer{
    text-align:center;
    background:#2e8b57;
    color:white;
    padding:15px;
    margin-top:20px;
}
// Mensagem de boas-vindas
window.onload = function () {
    alert("Bem-vindo ao site Campo e Cidade!");
};

// Muda a cor do título ao clicar
const titulo = document.querySelector("h1");

if (titulo) {
    titulo.addEventListener("click", function () {
        const cores = [
            "#2E8B57",
            "#FF9800",
            "#2196F3",
            "#9C27B0",
            "#E91E63"
        ];

        const corAleatoria =
            cores[Math.floor(Math.random() * cores.length)];

        titulo.style.color = corAleatoria;
    });
}

// Mostra a data e hora atual
function atualizarDataHora() {
    const elemento = document.getElementById("dataHora");

    if (elemento) {
        const agora = new Date();
        elemento.innerHTML =
            "Data e Hora: " + agora.toLocaleString("pt-BR");
    }
}

setInterval(atualizarDataHora, 1000);
