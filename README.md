# OpenPropMap

**Open source single-file interactive property tax & auction map.**

A fully self-contained HTML file built with Leaflet.js + Tailwind CSS. No backend, no dependencies beyond CDNs. Perfect for quick deployment, demos, internal tools, or as a starting template for county tax transparency portals.

## Live Demo

**https://5mil.github.io/open-property-map/**

## Features

- Interactive map centered on East Syracuse / Onondaga County, NY (easy to change)
- 12 sample properties with realistic tax data
- **Color-coded status**: Current (green), Delinquent (amber), Auction (rose)
- **Search by address or ZIP code** using OpenStreetMap Nominatim
- Click search result marker → "Show nearby properties" (within 3 miles, sorted by distance)
- Sidebar with live stats, filters, and searchable property list
- Detailed modal with tax history table and auction warnings
- Built-in JSON data editor (paste your own county data live)
- Export current data as JSON
- Fully responsive and keyboard accessible

## Quick Start

1. Download `index.html`
2. Open in any modern browser
3. Or host on GitHub Pages, Vercel, Netlify, or any static host

## Customize with Real Data

Click **"Edit Data"** in the app and replace the sample JSON array with your county's parcel + tax data.

Required fields per property:
- `id`, `address`, `lat`, `lng`, `status` ("Current" | "Delinquent" | "Auction"), `taxes_owed`

Recommended: `parcel_id`, `owner`, `property_type`, `assessed_value`, `annual_tax`, `auction_date`, `notes`

Many counties publish this data openly (GIS portals, assessor sites). Convert CSV/GeoJSON → JSON array and you're live.

## GitHub

- Repo: https://github.com/5mil/open-property-map
- Issues & contributions welcome!

## License

MIT / Public domain friendly — use it, fork it, improve it.

Built with ❤️ for open data and transparent government tools.