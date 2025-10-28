# Interactive Building Maps

A lightweight React + Leaflet application to create and explore custom interactive maps focused on buildings and polygons (not pins). Built with Tailwind CSS for styling.

Features
- Highlighted building outlines/polygons instead of pins
- Import GeoJSON (FeatureCollection / Feature)
- Click/select buildings to highlight boundaries
- Name, categorize, add descriptions, warnings, and images to each building
- Support for interior/nested buildings (link features as children)
- Filtering by type / tags
- Search by name, description, tags
- Local persistence using localStorage

Tech stack
- React (Vite)
- Leaflet + react-leaflet
- Tailwind CSS

Getting started
1. Install dependencies:
   npm install

2. Run dev server:
   npm run dev

Project structure (key files)
- src/App.jsx - application root, state
- src/components/MapView.jsx - Leaflet map + GeoJSON rendering
- src/components/Importer.jsx - GeoJSON import UI
- src/components/FeatureEditor.jsx - edit metadata, children (interior paths)
- src/utils/storage.js - localStorage helpers

Notes & next steps
- This demo supports GeoJSON import only. Add libraries like shpjs (for shapefiles) or topojson-client for other formats.
- Add image upload handling (currently uses image URLs).
- Add authentication and server-side storage for multi-user support.
- Add tile attribution, custom styles, and more map controls (draw/edit features).
- Add UX improvements: debounced search, bulk actions, and validation.

This repository is intended as a base to extend for building- and facility-focused mapping applications.