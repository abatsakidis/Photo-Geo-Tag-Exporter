# Photo Geo-Tag Exporter

A web application for extracting GPS metadata from images (JPEG with EXIF data and GeoTIFF files), previewing photos with their location on an interactive map, and exporting geospatial data in multiple formats.

---

## Features

- **Drag & Drop** or file select to upload multiple images simultaneously
- Preview of uploaded images alongside extracted GPS coordinates and metadata
- Supports reading GPS coordinates from:
  - **JPEG images with EXIF GPS data**
  - **GeoTIFF files with embedded geospatial info**
- Displays photo locations as markers on an interactive **Leaflet** map
- Export extracted data as:
  - **GeoJSON**
  - **KML**
  - **GeoPackage (GPKG)** — exported as a ZIP file containing GeoJSON for GIS software compatibility
- Metadata extraction includes:
  - Image capture date/time
  - Camera make and model (if available)
  - Coordinate system information for GeoTIFFs
- Basic coordinate system check and validation for GeoTIFF files

---

## How to Use

1. Open the `index.html` file in a modern web browser (Chrome, Firefox, Edge).
2. Drag & drop images (JPEG or GeoTIFF) onto the drop area or click it to select files manually.
3. Wait for the images to be processed:
   - A preview of each image will appear with GPS coordinates and metadata.
   - Locations will be shown on the interactive map.
4. Use the buttons below the drop area to download the collected location data in your preferred format:
   - **Download GeoJSON**
   - **Download KML**
   - **Download GeoPackage (ZIP)**
5. Import the exported files into GIS or mapping software as needed.

---

## Requirements

- A modern web browser with JavaScript enabled
- Internet connection to load Leaflet and external libraries via CDN (optional: download dependencies locally if needed)

---

## Notes

- Images without GPS metadata will be previewed but won't appear on the map or in the exports.
- GeoPackage export currently packages GeoJSON inside a ZIP archive for simplicity.
- Full native `.gpkg` file creation is not included but can be integrated with additional libraries if required.
- The application is purely client-side; no images or data are uploaded to any server.

---

## License

This project is open source and available for modification and redistribution.

---
