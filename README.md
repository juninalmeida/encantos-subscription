# 📚 Encantos Literários

Landing page de um clube de assinatura de livros, desenvolvida com foco em **CSS avançado**, **animações fluidas** e **responsividade mobile-first**.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-Mobile%20First-blueviolet?style=for-the-badge)

---

## 🎯 Sobre o Projeto

Uma landing page moderna para um serviço fictício de assinatura de livros. O projeto foi desenvolvido como exercício prático de **HTML e CSS avançado**, explorando técnicas modernas sem dependência de JavaScript.

### ✨ Destaques

- **Zero JavaScript** — Todas as interações são feitas puramente com CSS
- **Mobile-First** — Desenvolvido de 375px até 1024px+
- **Animações sofisticadas** — Mais de 20 keyframes customizados
- **CSS Moderno** — Uso de `:has()`, `animation-timeline`, `@supports`

---

## 🛠️ Técnicas CSS Utilizadas

### 🎨 Layout & Responsividade

| Técnica | Aplicação |
|---------|-----------|
| **Mobile-First** | Base em 375px, expandindo para tablets e desktop |
| **Flexbox** | Navbar, cards de pricing, footer |
| **CSS Grid** | Sobreposição de elementos na seção kit (`grid-area: 1/1`) |
| **`clamp()`** | Tipografia e espaçamentos fluidos |
| **`aspect-ratio`** | Proporções consistentes em backgrounds |

### ⚡ Animações Avançadas

```css
/* Scroll-Driven Animation (CSS Moderno) */
animation-timeline: view();
animation-range: entry 0% exit 100%;
```

- **Floating particles** — Partículas subindo nos botões
- **Staggered animations** — Delays sequenciais com `animation-delay`
- **SVG stroke animation** — Ícone do botão "desenhado" no hover
- **Highlight cycle** — Texto com brilho sequencial sincronizado

### 🎭 Interações sem JavaScript

```css
/* Seletor :has() para interação entre elementos */
.pricing-cards-container:has(.pricing-card:hover) .pricing-card--basic {
  opacity: 1;
  transform: translateX(0) rotate(-8deg);
}
```

- **Card fan effect** — Cards de pricing que "abrem em leque" no hover
- **Fold button** — Efeito de "dobra de página" no botão principal
- **Ripple effect** — Links sociais com pulso ao interagir

### 🔧 Recursos Modernos

| Recurso | Uso |
|---------|-----|
| `@supports` | Feature queries para fallbacks graceful |
| `inset` | Shorthand para posicionamento |
| CSS Custom Properties | Sistema de design tokens completo |
| `visibility` + `opacity` | Transições suaves mantendo acessibilidade |
| `pointer-events` | Controle de interatividade durante animações |

---

## 📁 Estrutura do Projeto

```
encantos-literarios/
├── index.html
├── styles/
│   ├── index.css          # Imports centralizados
│   ├── global.css         # Reset, variáveis, tokens
│   ├── hero.css           # Seção principal
│   ├── info-text.css      # Seção de descrição
│   ├── kit.css            # Showcase do kit mensal
│   ├── pricing.css        # Cards de preços
│   ├── footer.css         # Rodapé
│   └── animations.css     # Todas as @keyframes
└── assets/
    ├── logos/
    ├── icons/
    ├── images/
    ├── books/
    ├── backgrounds/
    └── desktop/
```

### 📐 Arquitetura CSS

O CSS está modularizado por **seções da página**, facilitando manutenção e escalabilidade:

- Cada arquivo contém os estilos base + media queries da sua seção
- `animations.css` centraliza todos os `@keyframes`
- `global.css` define o design system (cores, tipografia, espaçamentos)

---

## 🎨 Design System

### Paleta de Cores

```css
/* Cores principais */
--color-pink-base: #9547A5;
--color-blue-base: #358BB9;
--color-gold-base: #FFEB74;

/* Backgrounds */
--color-shape-background: #00050A;
--color-shape-base: #000F1F;
```

### Tipografia

- **Fonte:** Raleway (Google Fonts)
- **Escala:** De `0.625rem` (tags) até `3rem` (títulos)
- **Pesos:** 400 (regular), 500 (medium), 700 (bold)

---

## 📱 Breakpoints

| Breakpoint | Comportamento |
|------------|---------------|
| `< 376px` | Mobile base (design completo) |
| `376px - 1023px` | Tablet (animações simplificadas) |
| `≥ 1024px` | Desktop (interações hover ativadas) |

---

## 🚀 Como Executar

1. Clone o repositório
```bash
git clone https://github.com/juninalmeida/encantos-literarios.git
```

2. Abra o `index.html` no navegador

> 💡 Recomendo usar a extensão **Live Server** no VS Code para desenvolvimento

---

## 📸 Preview

### Mobile (375px)
Cards empilhados verticalmente com scroll-driven animations.

### Desktop (1024px+)
Cards em leque que se revelam no hover — efeito criado puramente com CSS usando `:has()`.

---

## 🧠 Aprendizados

Este projeto consolidou conhecimentos em:

- Arquitetura CSS escalável e modular
- Animações performáticas (usando `transform` e `opacity`)
- Progressive enhancement com `@supports`
- Interações complexas sem JavaScript
- Design responsivo verdadeiramente mobile-first

---

## 🔗 Links

- **Design (Figma):** [Rocketseat Community](https://www.figma.com/community/file/1394686421442995256/lp-de-clube-de-assinatura)

---

## 👤 Autor

**Júnior Almeida**

Desenvolvedor Full Stack em formação, focado em código limpo e escalável.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/júnior-almeida-3563a934b/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/juninalmeida)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:junioralmeidati2023@gmail.com)

---

## 📊 GitHub Stats

<div align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=juninalmeida&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=juninalmeida&layout=compact&langs_count=7&theme=tokyonight"/>
</div>

---

## 📄 Licença

Este projeto está sob a licença MIT. Desenvolvido como projeto PRÁTICO de estudos na trilha **Rocketseat**.

---

<div align="center">
  
  ⭐
  
</div>
