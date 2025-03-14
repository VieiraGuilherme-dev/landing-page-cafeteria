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

O arquivo `index.html` contém a estrutura principal da página, dividida em seções como **Sobre**, **Grãos** e **Contato**. Cada seção é acessível por meio de uma barra de navegação fixa.

~~~html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Café & Grãos</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="#about">Sobre</a></li>
        <li><a href="#grains">Grãos</a></li>
        <li><a href="#contact">Contato</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>Sobre</h2>
      <p>Saiba mais sobre nossa história e como escolhemos os melhores grãos.</p>
    </section>

    <section id="grains">
      <h2>Grãos</h2>
      <p>Descubra os tipos de grãos que oferecemos e suas origens.</p>
    </section>

    <section id="contact">
      <h2>Contato</h2>
      <p>Entre em contato conosco para mais informações sobre nossos produtos.</p>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Café & Grãos | Todos os direitos reservados.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
~~~

---

## 2. Estilização e Design Responsivo com CSS

Abaixo está o estilo da barra de navegação fixa e outras estilizações com **CSS3**.

~~~css
/* Estilo da barra de navegação */
nav ul {
  display: flex;
  justify-content: space-around;
  list-style: none;
}

nav a {
  text-decoration: none;
  color: #333;
  font-weight: bold;
  padding: 10px;
  transition: color 0.3s ease;
}

nav a:hover {
  color: #8B4513; /* Cor de destaque ao passar o mouse */
}
~~~

---

## 3. Interatividade com JavaScript

Abaixo está o código JavaScript que implementa a navegação suave entre as seções do site.

~~~javascript
// Código para navegação suave
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
  anchor.addEventListener('click', function (e) {
    e.preventDefault();

    document.querySelector(this.getAttribute('href')).scrollIntoView({
      behavior: 'smooth'
    });
  });
});
~~~

---

## 4. Responsividade

O site foi desenvolvido para ser responsivo, garantindo que a navegação e o layout se ajustem bem em dispositivos de diferentes tamanhos.

~~~css
/* Layout para telas pequenas */
@media (max-width: 768px) {
  nav ul {
    flex-direction: column;
    align-items: center;
  }

  section {
    padding: 20px;
  }
}
~~~

---

# 🚀 Como Rodar o Projeto Localmente

Para rodar este projeto localmente, siga as instruções abaixo:

1. **Clone o repositório:**

```bash
git clone https://github.com/seuusuario/cafe-e-graos.git
cd cafe-e-graos
