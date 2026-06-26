# NEXUS — Loja de Jogos 🎮

NEXUS é uma plataforma web moderna, responsiva e imersiva para a venda de chaves de ativação de jogos de PC, PlayStation, Xbox e Nintendo Switch. Construído com uma estética *cyberpunk/dark-neon* de alta fidelidade visual (com efeitos de *glassmorphism*), o projeto vai além de um simples e-commerce, integrando recursos avançados de gamificação, áudio e sincronização em nuvem.

[cite_start]O projeto padrão do Firebase vinculado a este repositório é o `nexus-4ed9e`[cite: 1].

---

## 🚀 Principais Funcionalidades

| Funcionalidade | Descrição |
| :--- | :--- |
| **Catálogo Interativo** | Filtros por gênero, plataforma, preço e relevância, além de busca em tempo real com sugestões. |
| **Carrinho e Checkout** | Sistema completo de precificação, suporte a cupons de desconto e simulação de gateway de pagamento. |
| **Autenticação de Usuários** | Criação de conta, login e persistência de sessão utilizando Firebase Authentication. |
| **Gamificação e Perfil** | Sistema de XP, progressão de níveis, conquistas desbloqueáveis, biblioteca de jogos e títulos customizáveis. |
| **Sincronização em Nuvem** | Integração com Firebase Firestore para salvar o progresso do usuário, lista de desejos e sistema de avaliações globais. |
| **Mini-games (Roda da Sorte)** | Roleta diária com *cooldown* para recompensar os usuários com experiência (XP) ou cupons de desconto exclusivos. |
| **Imersão Audiovisual** | Temas visuais dinâmicos, animações 3D nos cards (Tilt) e efeitos sonoros interativos construídos com a *Web Audio API*. |

---

## 🛠️ Tecnologias Utilizadas

* **Front-end:** HTML5 semântico, CSS3 (variáveis, transições, backdrop-filter) e JavaScript (Vanilla ES6+).
* **Back-end / BaaS:** Firebase (Hosting, Authentication, Firestore).
* **Ferramentas:** Node.js, `http-server` (para ambiente de desenvolvimento local).

---

## 📁 Estrutura do Projeto

A estrutura foi organizada seguindo as boas práticas do Firebase Hosting, centralizando os arquivos de produção na pasta `/public` (Single Source of Truth):

* **`/public/index.html`**: Estrutura principal, tags semânticas e acessibilidade.
* **`/public/style.css`**: Estilização global, temas customizados e micro-animações.
* **`/public/app.js`**: Lógica central de UI, gamificação, carrinho, áudio e integração Firestore.
* **`/public/auth.js`**: Gerenciamento de estado de usuário via Firebase Auth.
* **`/public/firebase-config.js`**: Credenciais e inicialização do SDK do Firebase.
* **`firebase.json`**: Diretrizes de deploy e comportamento de rotas de hospedagem.
* **`firestore.rules`**: Políticas e regras de segurança do banco de dados.

---

## 💻 Como Executar o Projeto Localmente

Certifique-se de ter o [Node.js](https://nodejs.org/) instalado em sua máquina.

1. Clone o repositório para sua máquina local.
2. Navegue até o diretório do projeto.
3. Instale as dependências (caso necessário) e inicie o servidor de desenvolvimento:
   ```bash
   npm run dev
