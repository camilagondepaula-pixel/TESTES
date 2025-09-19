<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Desfazer amizade com Camila</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
        background: linear-gradient(135deg, #ff3fa4, #ffd54f);
        color: #fff;
        height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    h1 {
        font-size: 2.5rem;
        margin-bottom: 10px;
    }
    p {
        font-size: 1.2rem;
    }
    button {
        padding: 10px 20px;
        font-size: 1rem;
        border: none;
        border-radius: 10px;
        background: #6a1b9a;
        color: #fff;
        cursor: pointer;
        position: relative;
    }
</style>
</head>
<body>

<h1>Boa sorte, Queridas!</h1>
<p>Mas... você quer desfazer a amizade?</p>
<button id="botao">Sim, quero desfazer amizade</button>

<script>
    const botao = document.getElementById('botao');

    botao.addEventListener('mouseover', () => {
        const x = Math.floor(Math.random() * (window.innerWidth - botao.offsetWidth));
        const y = Math.floor(Math.random() * (window.innerHeight - botao.offsetHeight));
        botao.style.position = 'absolute';
        botao.style.left = `${x}px`;
        botao.style.top = `${y}px`;
    });

    botao.addEventListener('click', () => {
        alert('Pegadinha! Você não vai se livrar de mim tão fácil');
    });
</script>

</body>
</html>
