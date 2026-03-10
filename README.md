# Writing Knowledge Graph

Interactive visualization of the K-12 Writing Instruction Knowledge Graph, based on the Writing Brainlift.

## View the Graph

Open `index.html` in a browser, or visit the GitHub Pages deployment.

## What This Is

A directed acyclic graph (DAG) of **156 Knowledge Components** across 3 strands and grades K-12, designed to power a mastery-based writing instruction app.

### Three Strands

| Strand | KCs | Color | Scope |
|--------|-----|-------|-------|
| **Composition** | 92 | Blue | Oral composition to sentences to paragraphs to essays to research papers |
| **Mechanics** | 40 | Green | Handwriting to spelling to contextual grammar to meaning-making to style |
| **Discourse** | 24 | Purple | Audience to voice to academic register to discipline-specific to publication |

### KC Types

Every node has a type that determines the activity the app should present:

- **Discrimination (D)** - Can the student SEE the problem? Always taught before Production.
- **Production (P)** - Can the student FIX or CREATE?
- **Structure (S)** - Does the student know the RULE?
- **Integrative (I)** - Can the student APPLY multiple skills in context?

### Gateway KCs

15 nodes are flagged as **Gateway KCs** (shown as red diamonds). If a student fails a gateway KC, all downstream learning is blocked. These are prioritized in the diagnostic system.

### Key Design Principles

- Discrimination always precedes Production for the same skill
- 80%+ mastery required before advancing
- Cross-strand connections are explicit (shown as gold dashed lines)
- Diagnostic entry points cascade through gateways to find any student's actual level in 3-5 probes

## Controls

- **Strand filters**: Toggle Composition / Mechanics / Discourse visibility
- **Grade filters**: Toggle K-2 / 3-5 / 6-8 / 9-12 visibility
- **Type filters**: Toggle D / P / S / I visibility
- **Gateways Only**: Show only the 15 gateway KCs
- **Hover** any node to see its details and connected prerequisites/dependents
- **Drag** nodes to rearrange
- **Scroll** to zoom, **click+drag** background to pan

## Files

| File | Description |
|------|-------------|
| `index.html` | Interactive D3.js visualization |
| `graph-data.json` | Complete graph data (156 nodes, 170+ edges) with all metadata |
| `README.md` | This file |

## Source

Based on the **Writing Brainlift** and the **MasteryWrite KC Framework**.
