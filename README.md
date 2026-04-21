# SoMAnTic - Social Media Analytics Tutorial

This is a project for the Web Information Systems course @ KU Leuven. 
An educational web platform and tutorial dashboard designed to help researchers navigate the complexities of gathering, querying, and analyzing data from various social media platforms using APIs.

---

## Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Research Modules](#research-modules)
- [Usage](#usage)
- [APIs Used](#apis-used)
- [Academic Context](#academic-context)
- [Requirements](#requirements)

---

## Overview

**SoMAnTic** (Social Media Analytics Tutorial) is a two-part web platform created to showcase approaches to social media analytics:

1. **Static Guidelines:** Explains what APIs are, the types of data they provide, and the limitations researchers face (including compliance with the European Digital Services Act).
2. **Live Query Showcase:** Demonstrates how posts can be queried and analyzed in real-time, utilizing various APIs to estimate demographics, parse linguistics, and fetch specific domain data.

This project was developed by Group G7 ("Almost Belgian") for the Web Information Systems course at KU Leuven.

---

## Project Structure

```text
./
├── CSS/                            # Global styling and KU Leuven Huisstijl
│   ├── main.css
│   └── showcase-styles.css
├── guidelines/                     # Static documentation and legal resources
│   ├── DSA.pdf
│   └── guidelines.html
├── research-showcase-pages/        # Interactive API demonstration modules
│   ├── about.html
│   ├── bluesky-keywords.html
│   ├── demographics.html
│   ├── football-pipeline.html
│   ├── linguistic-analysis.html
│   └── research-showcase-mainpage.html
├── index.js                        # Main application logic
├── package.json                    # Project dependencies
└── README.md                       # Project documentation
```

---

## Research Modules

The interactive portion of the site is divided into specific research tools. Each HTML file in the `research-showcase-pages` directory serves as a standalone module:

| Module | File | Description |
|---|---|---|
| **API Guidelines** | `guidelines.html` | Documentation on VLOPs, systemic risks, and API access forms. |
| **Demographics** | `demographics.html` | Predicts user age, gender, and nationality based solely on their first name. |
| **Linguistics** | `linguistic-analysis.html` | Automated parser for tokenization, tagging, and lemmatization of text. |
| **BlueSky Search** | `bluesky-keywords.html` | Live querying of the BlueSky social network using keyword parameters. |
| **Football Pipeline**| `football-pipeline.html` | Domain-specific data pipeline fetching live tables from global sports leagues. |

---

## Usage

Because this platform relies on vanilla HTML, CSS, and JavaScript, no complex build processes or backend servers are required to view it.

### Running Locally

1. Clone the repository:
```bash
git clone [https://github.com/petar-soldo/WIS-SoMAnTic.git](https://github.com/petar-soldo/WIS-SoMAnTic.git)
```
2. Navigate into the project folder:
```bash
cd WIS-SoMAnTic
```
3. Open the main showcase page in your browser:
```bash
# On Windows
start research-showcase-pages/research-showcase-mainpage.html

# On macOS
open research-showcase-pages/research-showcase-mainpage.html
```
*(Alternatively, you can open the folder in an IDE like WebStorm or VS Code and use a Live Server extension).*

---

## APIs Used

This project integrates several third-party APIs to demonstrate data retrieval and analysis:

* **Bluesky API:** Core social media querying (`docs.bsky.app`).
* **TheSportsDB API:** Fetching live football league data.
* **UDPipe API:** Multilingual linguistic analysis (`lindat.mff.cuni.cz`).
* **Demografix ApS:** Demographic estimations utilizing:
    * `nationalize.io`
    * `agify.io`
    * `genderize.io`

---

## Academic Context

* **Institution:** KU Leuven
* **Course:** Web Information Systems
* **Academic Year:** 2025-2026
* **Group:** G7 - "Almost Belgian"
* **Members:** * Victor Close (r1042528)
    * Aïcha David (r0833392)
    * Lisa D'Hoore (r1109614)
    * Petar Soldo (r1076709)

---

## Requirements

* A modern web browser (Chrome, Firefox, Edge, Safari) with JavaScript enabled.
* An active internet connection (required to fetch live data from the external APIs).