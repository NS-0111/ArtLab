 <div align="center">

# ArtLab — Interactive Digital Art Gallery

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![REST API](https://img.shields.io/badge/REST_API-005571?style=flat&logo=fastapi&logoColor=white)
![Met Museum](https://img.shields.io/badge/Metropolitan_Museum_API-333333?style=flat)

An interactive digital gallery for exploring artworks from the Metropolitan Museum of Art collection, featuring artwork search, catalog browsing and collection management.

</div>

---

## Table of Contents

- [About the Project](#about-the-project)
- [Key Features](#key-features)
- [Getting Started](#getting-started)
- [How It Works](#how-it-works)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Important Notes](#important-notes)
- [Limitations](#limitations)
- [License and Credits](#license-and-credits)
- [Development Team](#development-team)

---

## About the Project

ArtLab is an academic project developed for the Functional Programming course (COMP0393), with the goal of building an interactive digital art gallery using web technologies.

The application allows users to explore artworks, access information about different artists, and search the Metropolitan Museum of Art collection through its public API.

The project also implements artwork management operations and local data storage, providing an interactive experience for browsing and organizing the catalog.

## Key Features

- Digital art gallery featuring selected artworks.
- Integration with the Metropolitan Museum of Art public API.
- Artwork search based on collection-related terms.
- Artwork catalog displaying information such as title, artist, year and medium.
- Ability to add new artworks to the catalog.
- Artwork editing and deletion functionality.
- Local data storage using Local Storage.
- Caching mechanism to reduce unnecessary API requests.
- Timeline featuring different periods in art history.
- Development team showcase.

---

## Getting Started

### Prerequisites

- Modern web browser.
- Git.
- Python 3 or another local HTTP server.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/NS-0111/ArtLab.git
   ```

2. Navigate to the project directory:

   ```bash
   cd ArtLab
   ```

3. Start a local development server:

   ```bash
   python -m http.server 8000
   ```

4. Open the application in your browser:

   ```text
   http://localhost:8000
   ```

---

## How It Works

ArtLab uses JavaScript to control the interface, process searches, retrieve external data and manage information stored in the browser.

### Application Workflow

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
