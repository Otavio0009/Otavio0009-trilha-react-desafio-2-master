# 🔍 GitHub Wiki - Buscador de Repositórios

Aplicação web desenvolvida em **React** para buscar, listar e gerenciar repositórios públicos do GitHub em tempo real utilizando a **GitHub REST API**.

---

## ✨ Funcionalidades

- **Busca por Repositório:** Pesquisa direta utilizando o formato `usuario/nome-do-repositorio` (ex: `Otavio0009/CalculadoraReact`).
- **Prevenção de Duplicatas:** Verifica se o repositório já foi adicionado à lista antes de inseri-lo novamente.
- **Visualização Rápida:** Exibe o nome, o caminho completo (`full_name`) e um link direto para abrir o repositório no GitHub.
- **Remoção de Itens:** Permite remover repositórios da lista de exibição de forma dinâmica.
- **Tema Dark:** Interface estilizada com paleta escura inspirada no GitHub Dark Dimmed (`#22272e`).

---

## 🛠️ Tecnologias Utilizadas

- **ReactJS:** Biblioteca para construção da interface e gerenciamento de estado (`useState`).
- **Styled-Components:** Estilização CSS-in-JS componentizada e estilos globais (`createGlobalStyle`).
- **Axios:** Cliente HTTP utilizado para consumir os endpoints da API do GitHub (`https://api.github.com`).

---

## 📂 Estrutura do Projeto

```text
src/
├── assets/
│   └── github.png          # Logotipo do GitHub exibido no cabeçalho
├── components/
│   ├── Button/             # Componente de botão estilizado ("Buscar")
│   │   ├── index.js
│   │   └── styles.js
│   ├── Input/              # Campo de entrada de texto para busca
│   │   ├── index.js
│   │   └── styles.js
│   └── ItemRepo/           # Card de exibição e remoção de cada repositório encontrado
│       ├── index.js
│       └── styles.js
├── pages/
│   ├── App.js              # Página principal com a lógica de busca e listagem
│   └── styles.js           # Layout principal da aplicação
├── services/
│   └── api.js              # Configuração da instância do Axios (baseURL)
├── index.js                # Ponto de entrada da aplicação React
└── styles.js               # Definição de estilos globais (reset e cores base)
