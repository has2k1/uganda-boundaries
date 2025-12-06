# Administrative Boundaries of Uganda

This repository contains GeoJSON and GeoPackage files representing the administrative boundaries of Uganda at multiple hierarchical levels. The boundaries were extracted from UBOS's (Uganda Bureau of Statistics) interactive [dashboard](https://statistics.ubos.org/nphc/) for the 2024 National Population and Housing Census.

## Data Source and Quality

The boundaries are low-resolution versions and have been manually adjusted to correct several cartographic issues:
- Overlaps between adjacent territories
- Gaps between neighboring boundaries
- Incorrect administrative labels

**Note:** The adjustments were performed manually and are not reproducible through automated processes.

## Available Boundaries

The repository includes six administrative levels, available in both GeoJSON and GeoPackage formats in the `geojson/` and `gpkg/` directories:

### GeoJSON Format Files in the `geojson/` directory

1. **national.geojson** (~168 KB) - National boundary of Uganda
2. **regions.geojson** (~424 KB) - Regional boundaries (e.g., Central, Eastern, Western, Northern)
3. **subregions.geojson** (~848 KB) - Subregional divisions
4. **districts.geojson** (~2.7 MB) - District level boundaries
5. **counties.geojson** (~4.1 MB) - County level boundaries
6. **subcounties.geojson** (~11 MB) - Subcounty level boundaries (most detailed)

The GeoJSON files follow the standard GeoJSON specification with:
- Feature collections containing polygon geometries
- Properties including administrative names and codes
- WGS84 coordinate reference system (EPSG:4326)

### GeoPackage Format in the `gpkg/` directory

GeoPackage is an OGC standard, SQLite-based format that offers significant file size advantages:
All GeoPackage files use the same WGS84 coordinate reference system (EPSG:4326) as the GeoJSON versions and contain identical boundary data.

1. **national.gpkg** (~160 KB) - National boundary of Uganda
2. **regions.gpkg** (~262 KB)  - Regional boundaries (e.g., Central, Eastern, Western, Northern)
3. **subregions.gpkg** (~438 KB) - Subregional divisions
4. **districts.gpkg** (~1.3 MB) - District level boundaries
5. **counties.gpkg** (~2.0 MB) - County level boundaries
6. **subcounties.gpkg** (~5.9 MB) - Subcounty level boundaries (most detailed)

## Usage

These boundaries can be used for:
- Geographic analysis and mapping
- Spatial data visualization
- Administrative region identification
- Census data mapping and analysis
- GIS applications and web mapping services

## License

The data is derived from public census materials published by UBOS.
