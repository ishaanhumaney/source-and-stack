# Source & Stack

An independent, local-first web interface system designed for technical publications, engineering logs, and architectural diagnostics. This project skips the complex build toolchains to focus entirely on crisp typographic hierarchy, responsive asymmetric grid structures, and low-latency client-side rendering using vanilla semantic web components.

## Architecture Overview

Modern web design has largely outsourced its foundational layouts to massive JavaScript frameworks, introducing heavy client-side processing delays and dependency liabilities. Source & Stack takes the opposite approach. It serves as a proof-of-concept for content-heavy interfaces that require clean structural readability and zero infrastructure overhead.

The platform is divided into core operational vectors:
* **Core Stream (`index.html`):** The primary hub showing system data streams, perspective essays, and live network configurations.
* **Telemetry Grid (`telemetry.html`):** Deep-dive text layouts engineered for technical reading, complete with custom terminal/wireframe data slots.
* **Perspectives Sync (`perspectives.html`):** An opinion collection module utilizing clear text blocks and distinct author lines.
* **Network Node (`network.html`):** System configuration diagnostic lists displaying metadata variables cleanly.

## Key Features

* **Asymmetric Design System:** Deviates from predictable box layouts to create a high-impact, magazine-style layout flow.
* **Design Token Architecture:** Complete color palette, surface spacing variables, and font hierarchies are contained entirely within CSS variables inside `style.css` for instant global branding updates.
* **Zero Dependency Stack:** No Webpack, no Vite, no Tailwind layer, and no framework compilation steps. Pure browser-native runtime execution.
* **Fluid Responsive Adaption:** Uses CSS Grid columns combined with flexible flexbox components to change the viewport layout between mobile displays and wide workstation monitors.
* **Smooth Navigation Paths:** Internal anchors and page changes are linked via native smooth-scroll behaviors (`scroll-behavior: smooth`).

## Tech Stack Breakdown

* **Markup Language:** HTML5 (Semantic elements including `<header>`, `<main>`, `<article>`, `<section>`, `<footer>`)
* **Styling Engine:** CSS3 (Custom Variables, CSS Grid, Flexbox Layouts, Media Query Breakpoints)
* **Typography Vectors:** Google Fonts API integration fetching Space Grotesk (geometric headings) and DM Sans (high-legibility body text)

## Prerequisites & Browser Quick Start

Because this system runs completely raw, you don't even need to clone code to your local machine to edit or run it. 

### Option A: Cloud Development (GitHub Codespaces)
1. Near the top of this repository page, click the green **Code** button.
2. Select the **Codespaces** tab, then click **Create codespace on main**.
3. Once the browser terminal initializes, you can view the pages instantly by clicking **Go Live** on your status bar or running a simple server tool.

### Option B: Quick Local Launch
1. Download this repository as a `.zip` archive via the browser interface and extract it.
2. Open the project folder on your machine.
3. Double-click `index.html`. It will launch immediately in your preferred web browser without any local backend server dependencies.

## Project Structure

```text
source-and-stack/
├── .gitignore              # Development environment path exclusion rules
├── README.md               # System architectural documentation
├── index.html              # Main application portal & content stream
├── telemetry.html          # Deep-dive tech article layout matrix
├── perspectives.html       # Editorial commentary & opinion module
├── network.html            # Diagnostic hub and system data listing
└── style.css               # Core styling tokens, responsive grids & layout rules
```
## Roadmap
[ ] Theme State Toggle: Add native client-side JavaScript to cycle between high-contrast dark mode and amber-hued terminal styles.

[ ] Dynamic Search Indexing: Implement a dependency-free client-side search script utilizing browser memory pools to filter structural content blocks in real time.

[ ] RSS Feed Generation: Build an automated build-step script to parse semantic HTML data into compliant xml feeds for external network syndication.
