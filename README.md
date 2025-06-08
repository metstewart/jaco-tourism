# Jackson County Points of Interest Map

This is a Flask-based web application that displays a satellite map of Jackson County, Florida with interactive points of interest (POIs). Users can toggle a side menu to select POIs or click directly on map markers to view additional information in a modal at the bottom of the screen. The map also displays the county boundary overlay and uses custom marker icons by category.

## Features

-  Custom Google Maps pins for historic, recreational, and other categories
- Satellite map centered on Jackson County, FL
- Slide-out menu to view and navigate to POIs
- Zoom and pan to selected locations
- Description modal anchored to the bottom of the screen
- GeoJSON support for both POIs and county boundaries

## Tech Stack

- **Backend**: Flask
- **Frontend**: HTML, CSS, Vanilla JavaScript
- **Maps**: Google Maps JavaScript API
- **Data Format**: GeoJSON

## File Structure

```
/project-root
├── app.py                     # Flask application entry point
├── templates/
│   └── index.html             # Main HTML page with map and menu
├── static/
│   ├── style.css              # Styling for map and UI components
│   ├── jackson_county_pois.geojson  # GeoJSON file for POIs
│   └── jackson_boundary.json  # GeoJSON file for the Jackson County boundary
└── README.md                  # This file
```


## Customization

- To update or add POIs, modify `jackson_county_pois.geojson`.
- To adjust the boundary, modify `jackson_boundary.json`.
- Icons can be customized using different URLs or SVGs under the `icons` object in `index.html`.

