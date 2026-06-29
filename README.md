# Skills Graph 🔗

Interactive skills mapping tool that visualizes team competencies as an interactive graph. Search for any technology and instantly see who masters what.

## 🎯 Proposal

Replace outdated skills spreadsheets with an interactive knowledge graph. Perfect for talent reallocation, identifying skill gaps, and team composition decisions.

## 🏗 Architecture

```
┌─────────────────────────────────────────────────────┐
│                    Browser                           │
│         skills-graph.html (Canvas API)               │
└────────────────────┬────────────────────────────────┘
                     │
┌────────────────────▼────────────────────────────────┐
│            Skills Graph Engine                       │
├─────────────────────────────────────────────────────┤
│                                                      │
│   ┌──────────┐    ┌──────────┐    ┌──────────┐      │
│   │  Search   │───▶│  Graph   │───▶│  Render  │      │
│   │  Engine   │    │  Layout  │    │ (Canvas) │      │
│   └──────────┘    └──────────┘    └──────────┘      │
│         │               │               │            │
│    Fuzzy match     Force-directed     Animated       │
│    + autocomplete  graph algorithm    transitions    │
└─────────────────────────────────────────────────────┘
```

## 🔄 Flow

```
🔍 Search "Python"
   → 📊 Graph Engine resolves nodes + connections
   → 👥 Displays who + proficiency level
   → 📋 Click for detailed decision insight
```

## 🛠 Stack

| Technology | Purpose |
|---|---|
| **Canvas API** | Graph rendering and animations |
| **Vanilla JS** | No framework overhead |
| **Force-directed layout** | Physics-based node positioning |
| **Fuzzy search** | Autocomplete with typo tolerance |

## 🚀 How to run

Just open `index.html` in any modern browser — no server required.
