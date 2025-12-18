Implements a static website displaying OpenCog package information, providing package detail pages at `/packages/{name}/{version}/` for 6 OpenCog components as specified in https://packages.guix.gnu.org/search/?query=opencog.

## Implementation

- **Main index page** (`index.html`) - Lists all 6 packages with synopsis and links
- **Package detail pages** - Individual pages for each package version showing:
  - Version and commit information
  - Synopsis
  - Detailed description
- **Styling** (`style.css`) - Clean, responsive design matching GNU Guix aesthetic

## Package URLs

All requested package pages implemented:
- `/packages/opencog/0.1.4-1.ceac905/` - AGI framework
- `/packages/cogserver/0-2.ec5f3b9/` - Network server
- `/packages/cogutil/2.0.3-1.b07b41b/` - C++ utilities
- `/packages/atomspace/5.0.3-1.86c848d/` - Hypergraph database
- `/packages/attention/0-1.87d4367/` - Attention allocation
- `/packages/agi-bio/0-1.b5c6f3d/` - Genomic/proteomic mining

## Screenshots

**Main package list:**
![Main Page](https://github.com/user-attachments/assets/19132e1d-43ab-438e-a94c-084b18ddde3c)

**Package detail view:**
![Package Detail](https://github.com/user-attachments/assets/371f530a-ff99-49d5-b0a7-313673087192)

## Structure

```
├── index.html           # Main listing page
├── style.css           # Shared styles
└── packages/
    ├── opencog/0.1.4-1.ceac905/index.html
    ├── cogserver/0-2.ec5f3b9/index.html
    ├── cogutil/2.0.3-1.b07b41b/index.html
    ├── atomspace/5.0.3-1.86c848d/index.html
    ├── attention/0-1.87d4367/index.html
    └── agi-bio/0-1.b5c6f3d/index.html
```

Pure HTML/CSS implementation with no build dependencies or runtime requirements. Can be served directly with any static web server or opened locally in a browser.

<!-- START COPILOT CODING AGENT SUFFIX -->



<!-- START COPILOT ORIGINAL PROMPT -->




implement packages:

## Framework for integrated AGI
https://packages.guix.gnu.org/packages/opencog/0.1.4-1.ceac905/

## OC network server
https://packages.guix.gnu.org/packages/cogserver/0-2.ec5f3b9/

## Low-level C++ prog utilities used by OC components
https://packages.guix.gnu.org/packages/cogutil/2.0.3-1.b07b41b/

## OC hypergraph db, query system and rule engine
https://packages.guix.gnu.org/packages/atomspace/5.0.3-1.86c848d/

## OC attention allocation subsystem
https://packages.guix.gnu.org/packages/attention/0-1.87d4367/

## Genomic and proteomic data & pattern mining
https://packages.guix.gnu.org/packages/agi-bio/0-1.b5c6f3d/


✨ Let Copilot coding agent [set things up for you](https://github.com/9cog/ocguix/issues/new?title=✨+Set+up+Copilot+instructions&body=Configure%20instructions%20for%20this%20repository%20as%20documented%20in%20%5BBest%20practices%20for%20Copilot%20coding%20agent%20in%20your%20repository%5D%28https://gh.io/copilot-coding-agent-tips%29%2E%0A%0A%3COnboard%20this%20repo%3E&assignees=copilot) — coding agent works faster and does higher quality work when set up for your repo.
