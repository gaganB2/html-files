# Frontend Projects Portfolio

A collection of lightweight, high-performance web applications built with Vanilla JavaScript (ES6+), HTML5, and CSS3. 

Rather than relying on heavy frontend frameworks, these projects were architected to demonstrate rapid prototyping, system integration, and UI/UX planning. By utilizing modern development workflows, this portfolio showcases how to effectively connect external APIs, manage application state, and leverage specialized libraries to solve specific problems.

The primary focus areas of this repository are **Applied AI Integration** and **Data Visualization**.

## Technical Stack & Competencies
* **Core Technologies:** JavaScript (ES6+), HTML5, CSS3
* **Architecture & Integration:** REST API Integration, HTTP Streaming, Asynchronous Data Fetching, State Management (localStorage)
* **UI/UX Mechanics:** Intersection Observers, CSS Grid/Flexbox layouts, responsive design, data-driven DOM manipulation
* **Specialized Libraries:** Leaflet.js (GIS/Mapping), Three.js (WebGL rendering)

---

## Projects Overview

### 1. Local AI Chat Client
A zero-dependency chat interface designed to communicate directly with local Large Language Models (LLMs) via the Ollama REST API.
* **Live Demo:** Check its readme | **Source Code:** [/frontend_ollama_gemma](./frontend_ollama_gemma)
* **Architecture Highlights:**
  * Designed the integration layer to connect a web UI with a local LLM server.
  * Implemented ReadableStream to handle, parse, and render real-time text generation.
  * Built a parameter control panel allowing users to manipulate generation variables (Temperature, Top-P, Top-K, Context Size).
  * Handled session persistence using browser local storage.

### 2. NCRB Crime Data Dashboard
A public-facing analytical dashboard visualizing 2023 rape case data from the National Crime Records Bureau (NCRB).
* **Live Demo:** [https://r-pe-crimes.gagansahu55428.workers.dev/] | **Source Code:** [/rape_crime_dashboard](./rape_crime_dashboard)
* **Architecture Highlights:**
  * Planned and structured complex datasets into a clean, responsive CSS Grid layout.
  * Designed custom animated bar charts and metric cards utilizing pure CSS and DOM manipulation to avoid the overhead of heavy charting libraries.
  * Focused on responsible data presentation and clear visual hierarchy for public consumption.

### 3. Interactive Web Documentary (Manipur 2023)
A scroll-driven, interactive storytelling webpage detailing the 2023 ethnic violence in Manipur.
* **Live Demo:** [https://violence.gagansahu55428.workers.dev/] | **Source Code:** [/manipur_burning](./manipur_burning)
* **Architecture Highlights:**
  * Utilized the IntersectionObserver API to trigger narrative progression and UI state changes based on the user's scroll position.
  * Integrated Three.js to render a highly performant, WebGL-based atmospheric background effect.
  * Designed complex glassmorphism UI components to ensure text readability over dynamic backgrounds.

### 4. GIS Mapping Overlay (Balod District)
An interactive map overlay focusing on geographical boundaries and spatial data.
* **Live Demo:** [https://map-balod.gagansahu55428.workers.dev/] | **Source Code:** [/Map_balod](./Map_balod)
* **Architecture Highlights:**
  * Selected and integrated Leaflet.js for lightweight map rendering over OpenStreetMap and ESRI Satellite tiles.
  * Processed and rendered GeoJSON polygon data to accurately outline district boundaries.
  * Designed a custom, responsive floating UI panel to display location metadata.

### 5. Dynamic Quote Generator
An atmospheric web application that fetches and displays data asynchronously.
* **Live Demo:** [https://quote.gagansahu55428.workers.dev/] | **Source Code:** [/quote](./quote)
* **Architecture Highlights:**
  * Managed asynchronous external REST API fetching, including robust error handling and fallback UI states.
  * Planned and implemented mouse-tracking 3D CSS transforms (perspective, rotateX, rotateY) to create an interactive parallax layout.

---

## Local Development Instructions

These projects are built natively without build steps, bundlers, or package managers to ensure maximum portability and ease of deployment.

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git