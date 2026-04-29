# Artist Graphs: A Semantic Musicology Project

Welcome to **Artist Graphs**, a collaborative effort to map music history as a formal Knowledge Graph. This project treats band lineages, instrumentations, and "session-man" connections as structured data, ensuring high-fidelity mapping of the music industry from 1970 to the present.

## 🎸 Project Overview

This repository contains a collection of JSON-LD files, each representing a comprehensive knowledge graph for a specific band or artist. We use semantic technologies (Linked Data) to track:

*   **Band Lineups:** Precise membership windows and transitions.
*   **Musician Roles:** Detailed instrumental responsibilities and technical credits.
*   **Inter-Band Connections:** Relationships between musicians and the various groups they have been part of (e.g., Godley & Creme's transition from 10cc).
*   **Instruments:** A standardized vocabulary for musical instruments.

## 🛠 Semantic Architecture

Our data follows a strict ontological schema. Every entity and relation adheres to the following definitions:

*   **Namespace:** `music:` (`http://example.org/music/`)
*   **Classes:**
    *   `music:Band`: Includes `formedYear`, `activeYears`, `hasMember` (current), and `hadMember` (historical).
    *   `music:Musician`: Includes `hasRole`, `playsInstrument`, and reciprocal links (`isMemberOf`/`wasMemberOf`).
    *   `music:Instrument`: Declared as separate entities within the graph.

## 🤝 How to Contribute

We welcome contributions from fellow music historians and semantic tech enthusiasts! You can help by:

1.  **Adding New Artists:** Create a new JSON-LD file for a band or musician not yet covered. Use `10cc.json` as your master template.
2.  **Updating Information:** Improve the accuracy of existing graphs (e.g., adding a missing member, refining active years, or specifying a "session-man" role).
3.  **Reporting Errors:** Open an issue if you spot a factual or structural error in the data.

### Contribution Guidelines

*   **Ontological Rigidity:** Strictly follow the JSON-LD structure. Ensure all `@id` references are consistent.
*   **Structural Integrity:** Every `@graph` must be self-referential. If a band lists a member, that member must have a corresponding object in the same graph.
*   **Namespace Consistency:** Always use the `music:` prefix for domain-specific entities.

## 📊 Visualizations

You can view the interactive knowledge graphs for some of the bands in this collection here:

*   **10cc:** [View Graph](https://www.guitartabsexplorer.com/infograph/10cc)
*   **Metallica:** [View Graph](https://www.guitartabsexplorer.com/infograph/metallica)

## 🚀 Repository Link

Contribute and explore the data here:
**[https://github.com/adankert70/artistgraphs](https://github.com/adankert70/artistgraphs)**

---
*Mapping the DNA of music, one node at a time.*
