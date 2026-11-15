# ArtLab — Interactive Digital Art Gallery

An interactive digital gallery for exploring artworks from the Metropolitan Museum of Art collection, featuring artwork search, catalog browsing and collection management.

---

## Sumário

- [Sobre o projeto](#sobre-o-projeto)
- [Características principais](#características-principais)
- [Como executar](#como-executar)
- [Como funciona](#como-funciona)
- [Estrutura do projeto](#estrutura-do-projeto)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
- [Notas importantes](#notas-importantes)
- [Limitações](#limitações)
- [Licença e créditos](#licença-e-créditos)
- [Equipe de desenvolvimento](#equipe-de-desenvolvimento)

---

## Sobre o projeto

O ArtLab é um projeto acadêmico desenvolvido na disciplina de Programação Funcional (COMP0393), com o objetivo de criar uma galeria digital interativa utilizando tecnologias web.

A aplicação permite explorar obras de arte, consultar informações de diferentes artistas e pesquisar itens do acervo do Metropolitan Museum of Art por meio de sua API pública.

O projeto também implementa operações de gerenciamento de obras e armazenamento local, proporcionando uma experiência interativa de navegação e organização do catálogo.

## Características principais

- Galeria digital com apresentação de obras de arte.
- Integração com a API pública do Metropolitan Museum of Art.
- Pesquisa de obras por termos relacionados ao acervo.
- Catálogo com informações sobre título, artista, ano e técnica artística.
- Adição de novas obras ao catálogo.
- Edição e exclusão de obras cadastradas.
- Armazenamento local de dados utilizando Local Storage.
- Sistema de cache para reduzir requisições à API.
- Linha do tempo com diferentes períodos da história da arte.
- Interface para apresentação da equipe de desenvolvimento.

---

## Como executar

### Pré-requisitos

- Navegador web moderno.
- Git.
- Python 3 ou outro servidor HTTP local.

### Instalação

1. Clone o repositório:

   ```bash
   git clone https://github.com/NS-0111/ArtLab.git
   ```

2. Acesse o diretório:

   ```bash
   cd ArtLab
   ```

3. Inicie um servidor HTTP local:

   ```bash
   python -m http.server 8000
   ```

4. Acesse a aplicação pelo navegador:

   ```text
   http://localhost:8000
   ```

---

## Como funciona

O ArtLab utiliza JavaScript para controlar a interface, processar pesquisas, consultar dados externos e gerenciar as informações armazenadas no navegador.

### Fluxo de funcionamento

```text
ArtLab
   |
   ├── Homepage
   |     ├── Featured Artworks
   |     ├── Search
   |     └── Art History Timeline
   |
   ├── Art Catalog
   |     ├── Search Artworks
   |     ├── Add Artwork
   |     ├── Edit Artwork
   |     └── Delete Artwork
   |
   ├── Metropolitan Museum API
   |     ├── Search Collection
   |     └── Retrieve Artwork Details
   |
   └── Local Storage
         ├── User Collection
         └── Artwork Cache
```

### Etapas de processamento

| Etapa | Funcionamento |
|---|---|
| 1. Pesquisa | O usuário informa termos para localizar obras no catálogo |
| 2. Consulta à API | A aplicação envia requisições à API do Metropolitan Museum |
| 3. Recuperação | Os identificadores encontrados são utilizados para recuperar os detalhes das obras |
| 4. Cache | Os dados recuperados podem ser armazenados localmente para consultas futuras |
| 5. Exibição | As informações são renderizadas dinamicamente na interface |
| 6. Gerenciamento | O usuário pode adicionar, editar e excluir obras cadastradas localmente |

---

## Estrutura do projeto

```text
ArtLab/
│
├── assets/                  # Recursos visuais
│
├── css/
│   ├── homepage_ui.css       # Estilos da página inicial
│   ├── catalog_ui.css        # Estilos do catálogo
│   └── about_ui.css          # Estilos da página da equipe
│
├── src/
│   ├── homepage_ui.js        # Lógica da página inicial
│   ├── catalog_ui.js         # Lógica do catálogo
│   └── collection.js         # Gerenciamento de obras e armazenamento
│
├── index.html                # Página inicial
├── catalog.html              # Catálogo de obras
├── about.html                # Equipe de desenvolvimento
│
├── .editorconfig
├── .gitattributes
├── .gitignore
├── LICENSE
└── README.md
```

---

## Tecnologias utilizadas

| Tecnologia | Aplicação no projeto |
|---|---|
| HTML5 | Estruturação das páginas da aplicação |
| CSS3 | Estilização e organização visual da interface |
| JavaScript (ES Modules) | Lógica, interatividade e manipulação dinâmica do conteúdo |
| Fetch API | Comunicação assíncrona com serviços externos |
| Local Storage | Persistência local e armazenamento em cache |
| Metropolitan Museum API | Consulta ao acervo e recuperação de informações sobre obras |
| Git e GitHub | Versionamento e hospedagem do código-fonte |

---

## Notas importantes

- A aplicação utiliza a API pública do Metropolitan Museum of Art.
- As consultas externas dependem de conexão com a internet.
- O acesso à API utiliza um serviço de proxy para contornar restrições de CORS.
- As informações adicionadas pelo usuário são armazenadas no navegador por meio do Local Storage.
- O cache local permite reutilizar informações de obras já consultadas.

Documentação oficial: [Metropolitan Museum of Art Collection API](https://metmuseum.github.io/).

## Limitações

- A aplicação não possui backend ou banco de dados remoto.
- Os dados cadastrados pelo usuário ficam restritos ao armazenamento local do navegador.
- A disponibilidade das obras pesquisadas depende da API externa.
- A utilização do serviço de proxy introduz uma dependência de terceiros nas requisições externas.

---

## Licença e créditos

Este projeto utiliza a licença MIT, conforme especificado no arquivo [LICENSE](LICENSE).

Agradecimentos ao [Metropolitan Museum of Art](https://www.metmuseum.org/) pela disponibilização pública de seu acervo por meio da API de coleção.

## Equipe de desenvolvimento

Projeto desenvolvido colaborativamente por estudantes de Ciência da Computação da Universidade Federal de Sergipe (UFS).

| Integrante | GitHub |
|---|---|
| Anthony Levi T. dos Santos | [@aCube1](https://github.com/aCube1) |
| Nicolle Rillary Santana Silva | [@NS-0111](https://github.com/NS-0111) |
| Isaac Nascimento Santana | [@Isaacnsantana](https://github.com/Isaacnsantana) |
| Mateus Macedo Gonzaga | [@Mat-Macedo](https://github.com/Mat-Macedo) |

---

<p align="center">
  <strong>ArtLab</strong>
  <br />
  Exploring art through technology.
</p>
