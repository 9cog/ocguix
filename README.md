# ocguix

OpenCog Package Browser for GNU Guix

This repository contains a static website that displays information about OpenCog-related packages available in GNU Guix.

## Available Packages

- **opencog** (0.1.4-1.ceac905) - Framework for integrated AGI
- **cogserver** (0-2.ec5f3b9) - OC network server
- **cogutil** (2.0.3-1.b07b41b) - Low-level C++ prog utilities used by OC components
- **atomspace** (5.0.3-1.86c848d) - OC hypergraph db, query system and rule engine
- **attention** (0-1.87d4367) - OC attention allocation subsystem
- **agi-bio** (0-1.b5c6f3d) - Genomic and proteomic data & pattern mining

## Usage

This is a static website. To view it locally:

1. Clone the repository
2. Open `index.html` in a web browser
3. Or serve it with any web server (e.g., `python3 -m http.server`)

## GNU Guix Package Definition

The `opencog.scm` file contains the complete GNU Guix package definitions for all OpenCog components. To use these packages with GNU Guix:

1. Copy `opencog.scm` to your Guix channel or local package directory
2. Use it with `guix package -f opencog.scm` to install packages
3. Or add it to your Guix configuration

The file defines the following packages:
- `cogutil` - Low-level C++ utilities
- `atomspace` - Hypergraph database and rule engine
- `cogserver` - Network server
- `attention` - Attention allocation subsystem
- `opencog` - Main AGI framework
- `agi-bio` - Genomic and proteomic research tools

## Structure

- `index.html` - Main page with package list
- `style.css` - Styling for all pages
- `opencog.scm` - GNU Guix package definitions
- `packages/` - Directory containing individual package pages
  - `<package-name>/<version>/index.html` - Detail page for each package