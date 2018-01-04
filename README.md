# awesome-vector-tiles [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

The [Mapbox Vector Tile spec](https://www.mapbox.com/developers/vector-tiles/) is an efficient encoding for map
data into vector tiles that can be rendered dynamically.

### Parsers & Generators

- [vector-tile-js](https://github.com/mapbox/vector-tile-js) - Parses vector tiles with JavaScript.
- [mapnik-vector-tile](https://github.com/mapbox/mapnik-vector-tile) - C++ vector tile read/write implementation on top of Mapnik.
- [mbtiles-cpp](https://github.com/TimSC/mbtiles-cpp) - C++ library for decoding of mbtiles and vector data into function callbacks.
- [vector-tile-py](https://github.com/mapbox/vector-tile-py) - Python tool to convert a Mapnik vector tile to GeoJSON
- [node-mapnik](https://github.com/mapnik/node-mapnik) - Node.js API for vector tiles which depends on `mapnik-vector-tile`
- [vector-tile-cs](https://github.com/mapbox/vector-tile-cs) - Parses vector tiles with C# (native C# implementation, no dependencies).
- [mapbox-vector-tile-cs](https://github.com/bertt/mapbox-vector-tile-cs) - Parses vector tiles with C# (uses protobuf-net).
- [tilelive-bridge](https://github.com/mapbox/tilelive-bridge) - Implements [Tilelive API](https://github.com/mapbox/tilelive.js/blob/master/API.md) for creating vector tiles from traditional Mapnik datasources in Node.js.
- [tilelive-vector](https://github.com/mapbox/tilelive-vector) - Implements [Tilelive API](https://github.com/mapbox/tilelive.js/blob/master/API.md) for reading vector tiles and rendering to image tiles in Node.js.
- [mapbox-vector-tile](https://github.com/mapzen/mapbox-vector-tile) is a Python package for vector tile encoding maintained by Mapzen. (It is used in Mapzen's [vector tile service](http://mapzen.com/vector)).
- [geojson-vt](https://github.com/mapbox/geojson-vt) - Slice GeoJSON into vector tiles on the fly in the browser.
- [java-vector-tile](https://github.com/ElectronicChartCentre/java-vector-tile) - A java encoder and decoder for vector tiles.
- [mapbox-vector-tile-java](https://github.com/wdtinc/mapbox-vector-tile-java) - Encode and decode v2.1 Mapbox Vector Tiles. Convert JTS Geometry to and from MVT features, including simple user data support. Utility functions for converting world coordinates to MVT coordinates and clipping to a tile envelope.
- [cached-vector-tile](https://github.com/developmentseed/cached-vector-tile) - An alternative implementation of the vector-tile-js interface, backed by plain JS objects/arrays rather than parsed-on-demand protobuf data. Trades away memory efficiency for faster feature.loadGeometry() calls.
- [tilegrinder](https://github.com/rastapasta/tilegrinder) - A helper library for applying a data altering function on each vector tile in an MBTiles, using the native protobuf wrapper for de- and encoding, recompressing the results and storing them either in an MBTiles or as single files.
- [SwiftVectorTiles](https://github.com/manimaul/SwiftVectorTiles) - A Swift encoder for vector tiles according to the Mapbox vector tile spec.

## Clients

- [Mapbox GL Native](https://github.com/mapbox/mapbox-gl-native) - C++/OpenGL vector maps library with native SDKs for Android, iOS, Node.js, macOS, and Qt
- [Mapbox GL JS](https://github.com/mapbox/mapbox-gl-js) - JavaScript/WebGL vector maps library.
- [OpenLayers 3](https://github.com/openlayers/ol3/pull/4219) - JavaScript vector & raster library.
- [WhirlyGlobe/Maply](https://github.com/mousebird/WhirlyGlobe/blob/master/WhirlyGlobeSrc/WhirlyGlobe-MaplyComponent/src/MaplyMapnikVectorTiles.mm) - Objective C code that is able to read and render vector tiles(and style with mapnik xml) on iOS devices.
- [Leaflet.MapboxVectorTile](https://github.com/SpatialServer/Leaflet.MapboxVectorTile) is able to read PBF MapboxVectorTiles from a REST endpoint and render them as a TileLayer on a Leaflet Map. Use this option if you want to utilize vector tiles on a standard Leaflet web map without needing WebGL.
- [CARTO Mobile SDK](https://github.com/CartoDB/mobile-sdk) - C++ maps library focused on offline features, for iOS, Android, Windows Phone and Xamarin with bindings for Java, Objective-C and C#. Based on [Nutiteq Maps SDK](https://developer.nutiteq.com), but open source and uses CartoCSS.
- [Mapzen Tangram](https://github.com/tangrams/tangram) - JavaScript library for rendering 2D & 3D maps live in a web browser with WebGL, supports MVT, GeoJSON, TopoJSON
- [Mapzen Tangram-es](https://github.com/tangrams/tangram-es) - C++ library for rendering 2D and 3D maps using OpenGL ES 2 with custom styling and interactions
* [mapbox-gl-leaflet](https://github.com/mapbox/mapbox-gl-leaflet) - Create Mapbox GL layers in Leaflet
* [react-native-mapbox-gl](https://github.com/mapbox/react-native-mapbox-gl) - Render Mapbox GL maps from React applications
* [hoverboard](https://github.com/devTristan/hoverboard) - Render vector tiles on canvas with Leaflet 0.7.x (supports GeoJSON, TopoJSON, and protobuf)
* [Leaflet.VectorGrid](https://github.com/IvanSanchez/Leaflet.VectorGrid) - Display gridded vector data (sliced GeoJSON, TopoJSON or Mapbox Vector Tiles) in Leaflet 1.0.0
* [ArcGIS API for JavaScript](https://developers.arcgis.com/javascript/) - Draw vector tile layers as part of your web map. Rendering done via `mapbox-gl-js` integration.
* [mapscii](https://github.com/rastapasta/mapscii) - A Vector Tile to Braille and ASCII renderer for xterm-compatible terminals

### Applications / Command line tools

- [Mapbox Studio](https://github.com/mapbox/mapbox-studio) - Desktop design studio for both creating vector tiles from raw geodata and for rendering them on-the-fly into image tiles. Internally uses `tilelive.js` modules to handle vector tiles (see `tilelive-bridge` and `tilelive-vector`)
- [kosmtik](https://github.com/kosmtik/kosmtik) - Design maps with CartoCSS and Mapnik.
- [ArcGIS Pro](http://www.esri.com/en/software/arcgis-pro) - Generate vector tiles from maps authored in ArcGIS Pro or imported from ArcMap.
- [MVT Styler](http://sputnik-maps.github.io/mvt-styler/) - map style editor for vector tiles.
- [Maputnik](https://github.com/maputnik/editor) - A visual style editor for the Mapbox GL style specification.
- [QGIS Vector Tiles Reader](https://github.com/geometalab/Vector-Tiles-Reader-QGIS-Plugin) - QGIS Python plugin which reads Mapbox Vector Tiles from local MBTiles file or remote

## CLI Utilities

- [mbview](https://github.com/mapbox/mbview) - Watch MBTiles in your localhost. View tiles in a basic Mapbox GL JS webapp locally
- [MBUtil](https://github.com/mapbox/mbutil) - Import and export MBTiles to disk
- [Datamaps](https://github.com/ericfischer/datamaps) C application that can be used to create vector tiles and store them in an mbtiles. See the `render-vector` command.
- [tilemaker](https://github.com/systemed/tilemaker) - Command line tool to produce vector tiles directly from an .osm.pbf extract without an intermediate database.
- [vector-tiles-producer](https://github.com/vross/vector-tiles-producer) Command line tool in C++ to creates vector tiles for a given area at chosen zoom levels using a Mapnik XML.
- [tippecanoe](https://github.com/mapbox/tippecanoe) - Build vector tilesets from large collections of GeoJSON features.
- [vt-geojson](https://github.com/developmentseed/vt-geojson) - decodes vector tiles to GeoJSON FeatureCollections
- [tl](https://github.com/mojodna/tl) - An alternate command line interface to tilelive
- [tileshrink](https://github.com/rastapasta/tileshrink) - Reduce the layer extent and simplify the resulting geometries of all vector tiles in an MBTiles
- [tiler](https://github.com/Geovation/tiler) - Command line tool for converting GeoJSON, Shapefiles or PostGIS layer to raw Vector Tiles (or MBTiles)
- [geojson2mvt](https://github.com/NYCPlanning/geojson2mvt) - npm package for building a static vector tile tree for given xyz bounds from a geojson file (uses [geojson-vt](https://github.com/mapbox/geojson-vt))

## Mapbox GL JS Plugins

- [gl-draw](https://github.com/mapbox/gl-draw) - Adds support for drawing and editing features on Mapbox GL JS maps

## Servers

- [tessera](https://github.com/mojodna/tessera) - Supports serving and rendering vector tiles. Uses the same core libraries as Mapbox Studio.
- [tessella](https://github.com/urbica/tessella) - lightweight Node.js Mapbox Vector Tiles server. Inspired by tessera.
- [tilestrata](https://github.com/naturalatlas/tilestrata) - with tilestrata-vt, it can generate Mapnik Vector Tiles; with [tilestrata-postgismvt](https://github.com/Stezii/tilestrata-postgismvt), it can serve Mapbox Vector Tiles from a PostGIS db
- [Utilery](https://github.com/etalab/utilery) Server to generate vector tiles from PostGIS queries. Python based
- [tileserver](https://github.com/tilezen/tileserver) Mapzen Vector Tile Service.
- [TileStache](https://github.com/TileStache/TileStache) added support for Mapbox Vector tiles via .pbf extension requests.
- [Kartotherian](https://github.com/kartotherian/kartotherian) Wikipedia tile server with [Tilerator](https://github.com/kartotherian/tilerator) backend tile pre-generator
- [ArcGIS Online](http://www.esri.com/software/arcgis/arcgisonline) - Supports serving vector tiles and rendering in the mapping application powered by the ArcGIS API for JavaScript
- [Portal for ArcGIS](http://www.esri.com/software/arcgis/arcgisserver/extensions/portal-for-arcgis) - Supports serving vector tiles and rendering in the mapping application powered by the ArcGIS API for JavaScript
- [tilesplash](https://github.com/faradayio/tilesplash) - A light and quick nodejs webserver for serving topojson or mapbox vector tiles from a postgis backend
- [go-vtile-example](https://github.com/vicapow/go-vtile-example) - An example server written in Go
- [Tegola](https://github.com/terranodo/tegola) - A MVT server written in pure Go that supports serving tiles from a PostGIS data provider.
- [t-rex](https://github.com/pka/t-rex/) - MVT server in a single executable written in Rust. Serves tiles from PostGIS supporting custom tile grids.
- [postserve](https://github.com/openmaptiles/postserve) - A small Python based tileserver using ST_AsMVT and ST_AsMVTGeom to generate vector tiles on the fly. Designed for use with PostGIS 2.4 and the OpenMapTiles project
- [SpatialServer (PGRestAPI)](https://github.com/spatialdev/PGRestAPI) - A multi-purpose GeoSpatial NodeJS web server created at [SpatialDev](http://spatialdev.com) that not only serves MBTiles stuffed with vector tiles, it can also cut vector tiles on the fly from a PostGIS database. :warning: [_No longer maintained_](https://github.com/spatialdev/PGRestAPI/issues/142#issuecomment-231132808).
- [OpenMapTiles](https://github.com/openmaptiles) - Set of open-source tools for self-hosting of OpenStreetMap maps in more than 50 languages. It provides both raster as well as vector tiles, WMS and WMTS services for GIS programs, support for JavaScript viewers and mobile SDK.

## Low-level utilities

- [mapbox-gl-function](https://github.com/mapbox/mapbox-gl-function) - Mapbox GL style function evaluator
- [mapbox-gl-filter-simplify](https://github.com/mapbox/mapbox-gl-filter-simplify) - Simplifies and complexifies filters in Mapbox GL Styles
- [vt-pbf](https://github.com/anandthakker/vt-pbf) serialize JavaScript objects representing vector tiles into binary Protocol Buffer encodings of vector tiles
- [mvt-fixtures](https://github.com/mapbox/mvt-fixtures/) - a suite of valid and invalid test fixtures according to the Mapbox Vector Tile spec versions. Includes simplified unit test fixtures and real-world fixtures to test your encoders and decoders.

## Articles

- [Vector tiles remixed](http://gdunlop.github.io/Vector-tiles-remixed/) - guide to using [tilemaker](https://github.com/systemed/tilemaker) to generating vector tiles
- [Build Your Own Static Vector Tile Pipeline](https://geovation.github.io/build-your-own-static-vector-tile-pipeline) - guide transforming, encoding and hosting tiles in the cloud; using ogr2ogr + tippecanoe + Mapbox GL JS

## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Tom MacWright](http://macwright.org) has waived all copyright and related or neighboring rights to this work.
