# ArtLab — Digital Art Gallery

<p align="center">
  <strong>Discover. Explore. Create.</strong>
  <br />
  An interactive digital gallery designed to bring art closer to everyone.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-In%20Development-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" />
</p>

---

## Overview

**ArtLab** is a digital art gallery created to make artistic exploration more accessible and engaging.

The platform brings together an interactive art catalog, artwork discovery, and personal collection management, allowing users to explore masterpieces and build their own curated galleries.

Through integration with the **Metropolitan Museum of Art Collection API**, ArtLab provides access to artwork information and images from one of the world's most recognized art institutions.

## Features

- **Digital Art Gallery:** Explore a curated selection of artworks from different artistic periods.
- **Artwork Catalog:** Browse and discover artworks from the Metropolitan Museum of Art collection.
- **Smart Search:** Search for artworks using relevant terms, including titles and artists.
- **Personal Collection:** Add your own artworks to the catalog.
- **Artwork Management:** Edit and delete custom artwork entries.
- **Local Persistence:** Store personal collections and cached artworks using browser Local Storage.
- **Art History Timeline:** Discover important artistic periods throughout history.
- **Team Showcase:** Meet the people behind the project.

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure and semantic markup |
| CSS3 | Layout, styling and visual presentation |
| JavaScript (ES6+) | Application logic and interactivity |
| Web APIs | Browser functionality and Local Storage |
| Fetch API | Asynchronous communication with external services |
| Metropolitan Museum of Art API | Artwork data and image discovery |

### External Services

- [Metropolitan Museum of Art Collection API](https://metmuseum.github.io/) — Provides access to artwork records and collection information.
- [Google Fonts](https://fonts.google.com/) — Typography using the Inter font family.
- [CORS Proxy](https://corsproxy.io/) — Used to facilitate cross-origin API requests.

## Project Structure

```text
ArtLab/
│
├── assets/
│
├── css/
│   ├── homepage_ui.css
│   ├── catalog_ui.css
│   └── about_ui.css
│
├── src/
│   ├── homepage_ui.js
│   ├── catalog_ui.js
│   └── collection.js
│
├── index.html
├── catalog.html
├── about.html
│
├── .editorconfig
├── .gitattributes
├── .gitignore
├── LICENSE
└── README.md
```

## Getting Started

Follow these steps to run ArtLab locally.

### Prerequisites

You only need:

- A modern web browser.
- Git.
- Python 3 or another local HTTP server.

No additional package manager or build process is required.

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/NS-0111/ArtLab.git
```

**2. Navigate to the project directory**

```bash
cd ArtLab
```

**3. Start a local development server**

Using Python:

```bash
python -m http.server 8000
```

**4. Open the application**

Navigate to:

```text
http://localhost:8000
```

You can now explore the gallery and interact with its features.

## API Integration

ArtLab integrates with the Metropolitan Museum of Art Collection API to retrieve artwork information.

The application uses two main API endpoints:

| Endpoint | Description |
|---|---|
| `/search` | Searches the museum collection for matching artworks |
| `/objects/{objectID}` | Retrieves detailed information about a specific artwork |

The retrieved information includes:

- Artwork title.
- Artist name.
- Year of acquisition.
- Artistic medium.
- Artwork image URLs.

The application also implements a local caching mechanism to reduce unnecessary requests and improve the browsing experience.

For more information, visit the [official API documentation](https://metmuseum.github.io/).

## Data Persistence

ArtLab uses the browser's **Local Storage** to maintain artwork information between sessions.

Two storage categories are implemented:

- **User Collection:** Stores artworks manually added or modified by users.
- **Cache Collection:** Stores artwork information retrieved from the external API.

This approach allows the application to maintain a personal collection without requiring a dedicated backend or database.

> **Note:** Collections are stored locally in the browser. Clearing browser data or using another browser or device will not preserve the same collection.

## Project Goals

ArtLab was developed with the following goals:

- Encourage the exploration of art and cultural heritage.
- Provide an accessible digital environment for discovering artworks.
- Practice frontend development and JavaScript programming.
- Explore external API integration and asynchronous data retrieval.
- Apply CRUD operations and browser-based data persistence.
- Develop collaborative software engineering skills.

## Development Team

This project was developed collaboratively by Computer Science students at the Federal University of Sergipe.

| Contributor | GitHub |
|---|---|
| Anthony Levi T. dos Santos | [@aCube1](https://github.com/aCube1) |
| Nicolle Rillary Santana Silva | [@imnicolle](https://github.com/NS-0111) |
| Isaac Nascimento Santana | [@Isaacnsantana](https://github.com/Isaacnsantana) |
| Mateus Macedo Gonzaga | [@Mat-Macedo](https://github.com/Mat-Macedo) |

## License

This project is distributed under the **MIT License**.

See the [LICENSE](LICENSE) file for more information.

## Acknowledgements

Special thanks to:

- [The Metropolitan Museum of Art](https://www.metmuseum.org/) for making its collection data publicly accessible.
- The open-source community for the tools and resources that support projects like this.

---

<p align="center">
  <strong>ArtLab</strong>
  <br />
  <i>Where technology meets art.</i>
  <br /><br />
  Developed with curiosity, creativity and collaboration.
</p>
