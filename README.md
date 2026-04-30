# 🚗 CarrosFlix

Uma plataforma de streaming temática inspirada no universo do filme **Carros (Cars)** da Pixar, onde os usuários escolhem um perfil de personagem para acessar o catálogo de conteúdos.

---

## 📸 Visão Geral

O projeto simula uma tela de seleção de perfis no estilo Netflix, com os personagens **Relâmpago McQueen, Sally Carrera, Tow Mate e Finn McMissile**. Ao selecionar um perfil, o usuário é redirecionado para o catálogo personalizado.

---

## ✨ Funcionalidades

- Seleção de perfil com nome e avatar do personagem
- Redirecionamento para o catálogo após escolha do perfil
- Alternância entre **tema claro e escuro**
- Layout responsivo e acessível (uso de `role`, `aria-label`, `alt` nas imagens)

---

## 🗂️ Estrutura do Projeto

```
CarrosFlix/
│
├── index.html              # Página de seleção de perfis
├── style.css               # Estilos globais
├── theme-toggle.js         # Lógica de alternância de tema
│
├── assets/                 # Imagens dos perfis
│   ├── perfil_1.png        # Relâmpago McQueen
│   ├── perfil_2.png        # Sally Carrera
│   ├── perfil_3.png        # Tow Mate
│   └── perfil_4.png        # Finn McMissile
│
├── JavaScript/
│   └── index.js            # Lógica de seleção de perfil
│
└── catalogo/
    └── catalogo.html       # Página do catálogo de conteúdos
```

---

## 🛠️ Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript (Vanilla)

---

## 🚀 Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/carrosflix.git
   ```

2. Abra o arquivo `index.html` diretamente no navegador ou use uma extensão como o **Live Server** no VS Code.

> Nenhuma dependência ou instalação necessária.

---

## 🎨 Tema

O projeto conta com suporte a **modo claro e escuro**, alternado pelo botão no cabeçalho da página.
