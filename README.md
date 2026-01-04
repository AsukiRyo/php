# php

1. Criar pasta css e includes
2. Criar sidebar.php
3. Criar div sidebar
4. Colocar nome da aplicação
5. Criar links (Painel, Eventos...)
6. No CSS:
   - largura sidebar
   - altura 100vh
   - position fixed




conf o xampp
abrir a pasta do xampp
abrir "htdocs"
colocar o projeto na pasta "htdocs"

para testar o programa
abrir google e colar "http://localhost/eventflow2/index.php"





















https://www.w3schools.com/css/css_website_layout.asp
https://www.w3schools.com/css/css_positioning.asp
https://www.w3schools.com/php/php_includes.asp
https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps

index.php

<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <title>EventFlow</title>

    <!-- CSS principal -->
    <link rel="stylesheet" href="css/style.css">
</head>
<body>

    <?php include("includes/sidebar.php"); ?>

    <div class="content">
        <h2>Página Inicial</h2>
        <p>Sistema de gestão interna de eventos.</p>
    </div>

</body>
</html>




includes/sidebar.php


<div class="sidebar">

    <h1>EventFlow</h1>

    <a href="#">Painel</a>
    <a href="#">Eventos</a>
    <a href="#">Locais</a>
    <a href="#">Funcionários</a>

</div>




css/style.css

body {
    margin: 0;
    font-family: Arial, sans-serif;
}


.sidebar {
    width: 220px;
    height: 100vh;
    background-color: #ffffff;
    position: fixed;
    left: 0;
    top: 0;
}

.sidebar a {
    display: block;
    padding: 12px;
    text-decoration: none;
    color: #000;
}


.content {
    margin-left: 220px;
    padding: 20px;
}
