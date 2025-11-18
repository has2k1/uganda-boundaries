# Administrative Boundaries of Uganda

This repository contains GeoJSON files representing the administrative boundaries of Uganda at multiple hierarchical levels. The boundaries were extracted from UBOS's (Uganda Bureau of Statistics) interactive [dashboard](https://statistics.ubos.org/nphc/) for the 2024 National Population and Housing Census.

## Data Source and Quality

The boundaries are low-resolution versions and have been manually adjusted to correct several cartographic issues:
- Overlaps between adjacent territories
- Gaps between neighboring boundaries
- Incorrect administrative labels

**Note:** The adjustments were performed manually and are not reproducible through automated processes.

## Available Boundaries

The repository includes five administrative levels organized in the `geojson/` directory:

1. **national.geojson** (~200 KB) - National boundary of Uganda
2. **regions.geojson** (~188 KB) - Regional boundaries (e.g., Central, Eastern, Western, Northern)
3. **subregions.geojson** (~360 KB) - Sub-regional divisions
4. **districts.geojson** (~1.1 MB) - District-level boundaries
5. **counties.geojson** (~3.1 MB) - County-level boundaries (most detailed)

Each GeoJSON file follows the standard GeoJSON specification with:
- Feature collections containing polygon geometries
- Properties including administrative names and codes
- WGS84 coordinate reference system (EPSG:4326)

## Usage

These boundaries can be used for:
- Geographic analysis and mapping
- Spatial data visualization
- Administrative region identification
- Census data mapping and analysis
- GIS applications and web mapping services

## License

The data is derived from public census materials published by UBOS.
