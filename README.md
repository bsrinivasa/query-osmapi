Forked and built over [resolve-osm](https://github.com/batpad/resolve-osm) tool.
Acknowledgements: @batpad @planemad

# Query OSM API
Silly small package that takes a CSV file with `node_osm_id`, `way_osm_id` or `relation_osm_id` references to OpenStreetMap features and returns a valid GeoJSON.

Currently the script uses the osm_id and osm_type and queries for:
- lat
- long
- name
- name:zh
- wikidata
- wikipedia

Feel free to customise this script for the required fields. 

## Usage

Input csv should have `osm_id`, `osm_type`, and empty columns for the required fields.


Convert your CSV to a JSON

`csv2json foo.csv out.json`


Run the script

`node index.js <input_file.json> <output.geojson>`


