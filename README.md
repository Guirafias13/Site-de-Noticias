# 🎮 GeekNews - Portal de Cultura Pop e Tecnologia

O **GeekNews** é um site de notícias moderno e totalmente responsivo focado no ecossistema de cultura pop, games, tecnologia, cinema e animes. O projeto foi construído utilizando práticas modernas de desenvolvimento web focado em semântica estrutural, acessibilidade e alta performance de carregamento.

---

## 🚀 Funcionalidades Principais

* **Arquitetura Multi-página:** Navegação fluida entre a página principal (`index.html`), páginas internas de leitura completa e 4 portais específicos de categorias.
* **Sistema Dinâmico de Cores por Variáveis (`:root`):** Toda a identidade do site (bordas dos cards, etiquetas de marcação e efeitos hover no menu superior) adapta-se automaticamente à cor temática de cada categoria:
  * 🎬 **Filmes:** Vermelho (`#e52222`)
  * 🎮 **Games:** Azul (`#2d89ef`)
  * 💻 **Tecnologia:** Verde (`#00b37e`)
  * 🦊 **Animes:** Amarelo (`#c49d03`)
* **Acessibilidade e Contraste Otimizados:** Ajuste automatizado de contraste em etiquetas e botões para garantir uma taxa de legibilidade aprovada pelas diretrizes do Lighthouse (WCAG 2.1).
* **Mídia Otimizada e Responsiva:** Vídeos do YouTube acoplados de forma elástica, mantendo a proporção de cinema (16:9) e redimensionamento automático para celulares.
* **Monetização Realista:** Espaços inteligentes integrados para banners publicitários horizontais e responsivos sem quebra de layout.

---

## 🎨 Design e Layout

O portal adota o conceito de **Tema Escuro (Dark Mode)** profissional, utilizando cantos arredondados assimétricos e personalizados (`--curvatura: 10px 0 10px 0;`) e sombreamentos flutuantes para destacar os cartões de notícias.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estrutura semântica rigorosa utilizando as tags corretas (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<time>`, `<footer>`).
* **CSS3:** Estilização modular utilizando **CSS Grid** para a malha de notícias da Home e **Flexbox** para o alinhamento reto do rodapé e menus de navegação.

---

## ⚡ Otimizações de Performance (Lighthouse Core Web Vitals)

Para garantir uma pontuação máxima nos testes de carregamento, o projeto conta com as seguintes técnicas avançadas implementadas:
1. **Quebra de Caminho Crítico (Inlining CSS):** Injeção do estilo estrutural do topo direto no cabeçalho do HTML, eliminando o bloqueio de renderização (*Render-blocking requests*).
2. **Priorização de LCP via Preload:** Pré-carregamento explícito do banner principal com prioridade máxima (`fetchpriority="high"`), agilizando a pintura na tela.
3. **Economia de Bytes com Memória Cache:** Inclusão da propriedade `content-visibility: auto` nas fotos e anúncios para otimizar o processamento do navegador.

---

## 📂 Estrutura de Arquivos do Projeto

```text
Site de Noticias/
│
├── index.html                  # Página inicial (Home)
├── filmes.html                 # Categoria de Filmes
├── games.html                  # Categoria de Games
├── tecnologia.html             # Categoria de Tecnologia
├── animes.html                 # Categoria de Animes
├── style.css                   # Folha de estilos CSS definitiva
│
├── noticia_games1.html         # Matéria: The Witcher 4
├── noticia_games2.html         # Matéria: Sistema de Clima no GTA 6
├── noticia_vingadores.html     # Matéria: Trailer de Vingadores (Doom)
├── noticia_homem_aranha.html   # Matéria: Novo filme do Aranha
├── noticia_tecnologia.html     # Matéria: Inteligência Artificial de Voz
├── noticia_portateis.html      # Matéria: Chips para Consoles Portáteis
├── noticia_anime.html          # Matéria: Sequência de Chainsaw Man
└── noticia_dragonball.html     # Matéria: Nova saga de Dragon Ball
```

---

## 💻 Como Executar o Projeto

1. Baixe ou clone os arquivos para uma pasta no seu computador.
2. Certifique-se de ter uma subpasta chamada `img` contendo os arquivos de imagem das matérias e banners publicitários.
3. Dê um duplo clique no arquivo `index.html` para abrir o portal direto em qualquer navegador de internet.
4. Para simular e testar alterações em tempo real, use a extensão **Live Server** no VS Code.

---
Developed for study purposes in Web Development (HTML5 & CSS3). 🚀
