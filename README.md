header {
    background-color: #183C63;
    color: #FFFFFF;
    text-align: center;
    max-width: 800px;
    margin: 0 auto;
    padding: 16px;
}

main {
    background-color: #FFFFFF;
    color: #183C63;
    max-width: 800px;
    margin: 0 auto;
    padding: 16px;
}

article {
    display: flex;
}

img {
    width: 80px;
    height: 80px;
}

.artigo-autor {
    font-weight: bold;
}
<link rel="stylesheet" href="style.css">
const botoes = document.querySelectorAll("button");

botoes.forEach(function (botao) {
    let curtiu = false;
    botao.addEventListener("click", botaoClicado);
    function botaoClicado() {
        console.log("fui clicado");
        let texto = botao.querySelector("span");
        if (curtiu === false) {
            texto.textContent++;
            curtiu = true;
        } else {
            texto.textContent--;
            curtiu = false;
        }
    }
});
<script src="script.js"></script>
<article>
    <img src="imagem-blog.png" 
         alt="Descrição da imagem para acessibilidade">
    <div>
        <h2>Título da Nova Curiosidade</h2>
        <p class="artigo-autor">Por: Nome do Autor</p>
        <p>Texto da curiosidade tecnológica aqui.</p>
        <button>❤️<span>0</span></button>
        <button>��<span>0</span></button>
    </div>
</article>
<p>
Primeira parte do texto sobre computação.
<br><br>
Segunda parte do texto, que agora aparece em uma nova linha.
</p>
<p class="artigo-fonte">Fonte: The National Museum of Computing</p>
:root {
/* Nossas variáveis de cor ficarão aqui dentro */
}
:root {
    --cor-primaria: #183C63;
    --cor-secundaria: #3782d2;
    --cor-fundo: #ffffff;
    --cor-texto: #151428;
    --cor-contraste: #f3eef7;
    --cor-botao: #f9f9f9;
}
header {
    background-color: var(--cor-primaria);
}

main {
    background-color: var(--cor-fundo);
    color: var(--cor-texto);
}
    <!-- No arquivo index.html -->
    <body class="tema-escuro">
    /* No arquivo style.css */
    .tema-escuro {
    --cor-primaria: #c9e3ff; /* Um azul mais claro para destacar no fundo escuro */
    --cor-fundo: #151428;    /* Fundo escuro */
    --cor-texto: #ffffff;   /* Texto branco */
    /* Continue invertendo as cores conforme o seu layout */
}
.tema-escuro a {

}
.tema-escuro a {
    color: var(--cor-secundaria);
}
.tema-escuro p {

}
.tema-escuro p {
    color: var(--cor-texto);
}
.tema-escuro header p {

}
.tema-escuro header p {
    color: var(--cor-contraste);
}
--fonte-texto:
body {
    max-width: 100vw;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
body {
    max-width: 100vw;
    font-family: 'Segoe UI', sans-serif;
}
body {
    max-width: 100vw;
    font-family: var(--fonte-texto);
}
--fonte-texto: 'Segoe UI', sans-serif;