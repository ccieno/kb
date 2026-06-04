# kb — Demo Knowledge Bases

A GitHub Pages site hosting demo knowledge base content for multiple industries. Used to demonstrate Zoom Contact Centre's AI knowledge base and self-service capabilities during sales demos.

**Deployed at:** `kb.eno.solutions` (via CNAME)

## What it does

Provides a library of realistic, industry-specific knowledge base articles and documents that can be indexed by ZCC's AI engine or linked directly from a ZCC flow. Each vertical has its own subfolder with HTML articles and/or PDFs.

## Industry verticals

| Vertical | Content |
|---|---|
| `hotels/` | PDF property guides for various hotel locations (London, Glasgow, Maldives, Seychelles, etc.) |
| `nhs/` | HTML patient information articles (stitches care, going home, parking, catering, mobile phones, etc.) |
| `retail/` | PDF product guides |
| `dental/` | Dental practice content |
| `bakers/` | Bakery/food service content |
| `insurance/` | Insurance product content |
| `legal/` | Legal services content |
| `articles/` | Cross-vertical articles (appointments, retail) |

## Structure

```
kb/
├── index.html          # Landing page with links to each vertical
├── hotels/             # Hotel property PDFs
├── nhs/                # NHS patient info HTML articles + CSV article index
├── retail/             # Retail product PDFs
├── dental/             
├── bakers/             
├── insurance/          
├── legal/              
└── articles/           
```

## How to use in a demo

Point the ZCC Knowledge Base configuration to any article URL on this site (e.g. `https://kb.eno.solutions/nhs/stitches.html`). The AI will index and answer questions based on the content. Switch verticals by updating the knowledge base source URL in the ZCC admin.

## Deployment

Static files served via GitHub Pages. Push changes to `main` and they're live automatically.
