# freshbond-map

Map tiles for the FreshBond app's Keşfet map: one PMTiles file of Turkey,
cut from the Protomaps daily basemap build with `pmtiles extract`, served by
GitHub Pages.

Map data © OpenStreetMap contributors (ODbL). Basemap schema by Protomaps.

`turkey.pmtiles`: Protomaps build 2026-09-25, cut to Turkey's border
(geoBoundaries ADM0, simplified), zoom 0–11, about 85 MB. Rebuild:

    pmtiles extract https://build.protomaps.com/<YYYYMMDD>.pmtiles turkey.pmtiles \
      --region=tur_adm0.geojson --maxzoom=11
