# 🚗 CarrosFlix

Uma plataforma de streaming temática inspirada no universo do filme **Carros (Cars)** da Pixar, que simula uma experiência estilo Netflix — com seleção de perfis, catálogo de conteúdos e reprodução de trailers em hover.

---

## 📸 Visão Geral

O projeto é composto por duas telas principais:

- **Tela de perfis (`index.html`):** o usuário escolhe entre os personagens Relâmpago McQueen, Sally, Mate e Finn para acessar o catálogo.
- **Catálogo (`catalogo.html`):** exibe carrosséis de conteúdo organizados por categoria, com cards interativos que reproduzem trailers do YouTube ao passar o mouse.

---

## ✨ Funcionalidades

- Seleção de perfil com nome e avatar salvos via `localStorage`
- Catálogo gerado dinamicamente a partir de dados em `data.js`
- Cards com **reprodução automática de trailer** (YouTube embed) ao hover
- Modal de detalhes com score de relevância, classificação etária, duração e tags
- Barra de progresso de visualização nos conteúdos em andamento
- Expansão dos cards com ajuste de origem para evitar corte nas bordas
- Alternância entre **tema claro e escuro**
- Layout responsivo

---

## 🗂️ Estrutura do Projeto

```
CarrosFlix/
│
├── index.html                  # Tela de seleção de perfis
├── style.css                   # Estilos da tela de perfis
├── theme-toggle.js             # Lógica de alternância de tema
│
├── assets/                     # Avatares dos perfis
│   ├── perfil_1.png            # Relâmpago McQueen
│   ├── perfil_2.png            # Sally Carrera
│   ├── perfil_3.png            # Tow Mate
│   └── perfil_4.png            # Finn McMissile
│
├── JavaScript/
│   └── index.js                # Salva perfil selecionado no localStorage
│
└── catalogo/
    ├── catalogo.html           # Página do catálogo
    ├── catalogo.css            # Estilos do catálogo
    └── js/
        ├── main.js             # Ponto de entrada — renderiza os carrosséis
        ├── data.js             # Dados das categorias e itens do catálogo
        ├── utils.js            # Funções utilitárias (YouTube ID, badges, etc.)
        └── components/
            ├── Carousel.js     # Componente de carrossel por categoria
            └── Card.js         # Componente de card com hover e trailer
```

---

## 🧩 Arquitetura

O catálogo é construído de forma modular com JavaScript puro (ES Modules):

- **`data.js`** — define as categorias e os itens (imagem, link do YouTube, progresso, badges)
- **`main.js`** — aguarda o DOM carregar, recupera o perfil do `localStorage` e renderiza os carrosséis
- **`Carousel.js`** — cria a seção de cada categoria com título e fileira de cards
- **`Card.js`** — cria cada card com lógica de hover, embed de trailer, barra de progresso e modal de detalhes
- **`utils.js`** — funções auxiliares: extrair ID do YouTube, gerar score aleatório, duração e classificação etária

---

## 🛠️ Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript ES6+ (Módulos nativos, sem frameworks)
- YouTube IFrame API (embed com autoplay)
- Font Awesome (ícones)
- Google Fonts (Roboto)

---

## 🚀 Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/carrosflix.git
   ```

2. Abra com o **Live Server** no VS Code (recomendado), pois o projeto usa ES Modules (`type="module"`), que não funcionam via `file://` no navegador.

> Nenhuma dependência ou instalação necessária.

---

## 🎨 Tema

O projeto conta com suporte a **modo claro e escuro**, alternado pelo botão no cabeçalho da tela de perfis.
