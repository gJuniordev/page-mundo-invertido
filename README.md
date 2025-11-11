# 🌍 Projeto Mundo Invertido (Stranger Things Theme Switcher)

![Badge de Tecnologia: HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Badge de Tecnologia: CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Badge de Tecnologia: JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

Um projeto didático para demonstrar a alternância de temas (Light/Dark Mode) usando **variáveis CSS** e manipulação de classes com **JavaScript**, inspirado na série Stranger Things.

## ✨ Funcionalidades Principais

* **Alternância de Tema:** Clique no botão "Inverter Mundos" para trocar instantaneamente o visual da página entre o **Tema Claro (Mundo Normal)** e o **Tema Escuro (Mundo Invertido)**.
* **Design Responsivo:** (Se o seu código for responsivo) O layout é adaptado para diferentes tamanhos de tela.
* **Efeitos do Mundo Invertido:** Aplicação de fontes diferenciadas e transformações CSS (`rotateZ(180deg) scaleX(-1)`) em elementos específicos.

## ⚙️ Como Funciona a Troca de Tema

O coração da funcionalidade está em três partes:

### 1. HTML (O Gatilho)

O botão chama a função JavaScript `switchTheme()` ao ser clicado.

```html
<button id="switch-theme-button" onclick="switchTheme()">Inverter Mundos</button>
```

### 2. JavaScript (A Ação)
A função switchTheme() usa o método .toggle() para alternar as classes dark-theme e light-theme no elemento <body>.

```javascript
function switchTheme() {
    document.body.classList.toggle('dark-theme');
    document.body.classList.toggle('light-theme');
}
```

### 3. CSS (O Estilo)
O CSS define dois blocos de estilos, .light-theme e .dark-theme, que usam Variáveis CSS (--) para armazenar as configurações de cores, fundos e imagens. Quando o JavaScript troca a classe no <body>, todo o layout se ajusta automaticamente para usar os valores do tema ativo.

```css
/* Exemplo de Variáveis no Tema Escuro */
.dark-theme {
  --page-background: linear-gradient(...);
  --highlight-color: #ffffff; /* Letras Brancas */
  --featured-font-family: "Rubik Glitch", sans-serif;
}

/* Aplicação de efeito especial */
.dark-theme .invert-element {
    transform: rotateZ(180deg) scaleX(-1);
}
```

## 🛠️ Tecnologias Utilizadas

- HTML5: Estrutura da página.
- CSS3: Estilização e definição das variáveis de tema.
- JavaScript: Lógica para a alternância de classes (.toggle()).

## 📥 Como Rodar o Projeto
Você pode rodar este projeto localmente em seu computador seguindo os passos:

### Clone o Repositório:

```
git clone (https://github.com/gJuniordev/page-mundo-invertido.git)
```
### Navegue até a pasta:
```
cd mundo-invertido-landing-page
```
## 📸 Preview

<img width="1867" height="881" alt="image" src="https://github.com/user-attachments/assets/ec8ec043-1022-4436-99ca-f0fc1af8740c" />

<img width="1866" height="879" alt="image" src="https://github.com/user-attachments/assets/d0105a1c-2844-4709-a964-a103cc8550ef" />

## 🎓 Contexto Educacional
Este projeto foi desenvolvido como parte da **Formação CSS Web Developer** da [DIO.me](https://www.dio.me), com o objetivo de praticar.

## 👨‍💻 Autor
**Gilcélio Júnior - Juntamente a DIO.ME**
- 💼 [LinkedIn](https://www.linkedin.com/in/gilc%C3%A9lio-j%C3%BAnior-ab032924a/)
- 🐙 [GitHub](https://github.com/gJuniordev)

