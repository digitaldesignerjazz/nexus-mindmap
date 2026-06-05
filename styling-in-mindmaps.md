# Styling Mindmaps in Mermaid

Mindmaps support `classDef` and `class` but with some limitations compared to flowcharts.

## Recommended Pattern

```mermaid
mindmap
  root((NEXUS))
    AI
    Mesh
    Blockchain

classDef core fill:#1e3a5f,color:#fff,stroke:#38bdf8,stroke-width:3px
classDef pillar fill:#0f172a,color:#e0f2fe,stroke:#64748b
class root core
class AI,Mes h,Blockchain pillar
```

## Color Strategy

- Use a cohesive palette (deep blues, cyans, golds)
- Differentiate the root node strongly
- Give each major branch its own subtle color family

## Limitations

Mindmaps have fewer styling options than flowcharts. For very complex visual hierarchies, consider using a flowchart with subgraphs instead.