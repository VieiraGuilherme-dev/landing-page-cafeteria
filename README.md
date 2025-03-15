<p align="center"> 
  <img src="https://readme-typing-svg.herokuapp.com?font=Century+Gothic&weight=800&size=48&pause=1000&color=F7F7F7&center=true&vCenter=true&width=600&lines=Site+de+Café+e+Grãos" alt="Typing SVG" />
</p>

---

# 📖 Visão Geral

Este projeto é um site para a **Cafeteria Café & Grãos**, desenvolvido com foco em apresentar uma experiência agradável aos amantes de café. O site foi criado com **HTML5**, **CSS3** e **JavaScript**, sendo totalmente responsivo para garantir acessibilidade e navegação fluida em qualquer dispositivo. O projeto é ideal para quem busca informações sobre os diferentes tipos de grãos de café e métodos de preparo. ☕✨

---

# 🌟 Funcionalidades e Destaques

- **Design Responsivo:** O layout do site é responsivo e adaptável a diferentes tamanhos de tela, proporcionando uma ótima experiência em dispositivos móveis, tablets e desktops. 📱💻

- **Navegação Suave:** Utilizamos **JavaScript** para garantir que a navegação entre as seções do site seja suave, sem a necessidade de recarregar a página.

- **Interatividade com JavaScript:** O site possui funcionalidades dinâmicas, como a navegação entre seções, animações e interações com o usuário.

- **Estilização Moderna:** O uso de **CSS3** garante um design simples, mas elegante, com animações e transições suaves que melhoram a experiência do usuário.

- **Barra de Navegação Fixa:** A barra de navegação fixa oferece fácil acesso às principais seções do site: **Sobre**, **Grãos** e **Contato**. ☕🛒

---

# 🛠️ Tecnologias Utilizadas

<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" height="35"  />

• Estruturação do conteúdo e organização da página.

##

<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" height="35"  />

• Estilização moderna e responsiva, com animações e transições para um design atraente.

##

<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" height="35"  />

• Implementação de interatividade e navegação dinâmica entre as seções do site.

---

# 📂 Estrutura do Projeto e Detalhes de Implementação

## 1. Composição do Site (index.html)

O arquivo `index.html` contém a estrutura principal da página, dividida em seções como **Home**, **Sobre**, **Menu**, **Avaliações** e **Endereço**. Cada seção é acessível por meio de uma barra de navegação fixa.

~~~html
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@500&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@700&display=swap" rel="stylesheet">
    <title>Caffè & Grão</title>
</head>

<body>
    <header class="header">
        <section>
            <a href="#" class="logo">
                <img src="./img/logo.png" alt="logo">
            </a>

            <nav class="navbar">
                <a href="home">Home</a>
                <a href="about">Sobre</a>
                <a href="menu">Menu</a>
                <a href="review">Avaliações</a>
                <a href="address">Endereço</a>
            </nav>

            <div class="icons">
                <img width="30" height="30" src="https://img.icons8.com/ios-filled/30/ffffff/search--v1.png"
                    alt="search--v1" />
                <img width="30" height="30" src="https://img.icons8.com/material/30/ffffff/shopping-cart--v1.png"
                    alt="shopping-cart--v1" />
            </div>
        </section>
    </header>
~~~

---

## 2. Estilização e Design Responsivo com CSS

Abaixo está o estilo da barra de navegação fixa e outras estilizações com **CSS3**.

~~~css
.header{
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 99;
    border-bottom: var(--border);
    background-color: var(--bg);
}

.header section{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-top: 1.5rem;
    padding-bottom: 1.5rem;
}

.navbar a{
    color: #fff; 
    font-size: 1.8rem;
    letter-spacing: 0.1rem;
    margin-right: 2rem;
}

.navbar a:hover{
    color: var(--main-color);
    border-bottom: 0.1rem solid var(--main-color);
    padding-bottom: 0;
    font-size: 2rem;
}


~~~

---

## 3. Interatividade com JavaScript

Abaixo está o código JavaScript que implementa a navegação suave entre as seções do site.

~~~javascript

document.addEventListener('DOMContentLoaded', function () {
    const links = document.querySelectorAll('nav ul li a');

    links.forEach(link => {
        link.addEventListener('click', function (e) {
            e.preventDefault();

            const targetId = this.getAttribute('href').substring(1);

            const targetSection = document.getElementById(targetId);
            targetSection.scrollIntoView({
                behavior: 'smooth',
                block: 'start'
            });
        });
    });
});
~~~

---

## 4. Responsividade

O site foi desenvolvido para ser responsivo, garantindo que a navegação e o layout se ajustem bem em dispositivos de diferentes tamanhos.

~~~css
*{
    margin: 0;
    padding: 0;
    outline: none;
    border: none;;
    text-decoration: none;
    text-transform: capitalize;
    transition: 0.2s linear;
    font-family: "Roboto", sans-serif;
}

body{
    background-color: var(--bg);
}

section{
    padding: 3rem 2rem;
    margin: 0 auto;
    max-width: 1200px;
}
~~~

---

# 🚀 Como Rodar o Projeto Localmente

Para rodar este projeto localmente, siga as instruções abaixo:

1. **Clone o repositório:**

```bash
git clone https://github.com/seuusuario/cafe-e-graos.git
cd cafe-e-graos
