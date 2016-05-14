# awesome-vector-tiles [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

The [Mapbox Vector Tile spec](https://www.mapbox.com/developers/vector-tiles/) is an efficient encoding for map
data into vector tiles that can be rendered dynamically.

### Parsers & Generators

- [vector-tile-js](https://github.com/mapbox/vector-tile-js) - Parses vector tiles with JavaScript.
- [mapnik-vector-tile](https://github.com/mapbox/mapnik-vector-tile) - C++ vector tile read/write implementation on top of Mapnik.
- [vector-tile-py](https://github.com/mapbox/vector-tile-py) - Python vector tile decoder implementation
- [node-mapnik](https://github.com/mapnik/node-mapnik) - Node.js API for vector tiles which depends on `mapnik-vector-tile`
- [mapbox-vector-tile-cs](https://github.com/bertt/mapbox-vector-tile-cs) - Parses vector tiles with C#.
- [tilelive-bridge](https://github.com/mapbox/tilelive-bridge) - Implements [Tilelive API](https://github.com/mapbox/tilelive.js/blob/master/API.md) for creating vector tiles from traditional Mapnik datasources in Node.js.
- [tilelive-vector](https://github.com/mapbox/tilelive-vector) - Implements [Tilelive API](https://github.com/mapbox/tilelive.js/blob/master/API.md) for reading vector tiles and rendering to image tiles in Node.js.
- [mapbox-vector-tile](https://github.com/mapzen/mapbox-vector-tile) is a Python package for vector tile encoding maintained by Mapzen. (It is used in Mapzen's [vector tile service](http://mapzen.com/vector)).
- [geojson-vt](https://github.com/mapbox/geojson-vt) - Slice GeoJSON into vector tiles on the fly in the browser.
- [java-vector-tile](https://github.com/ElectronicChartCentre/java-vector-tile) - A java encoder and decoder for vector tiles.

## Clients

- [Mapbox GL Native](https://github.com/mapbox/mapbox-gl-native) - C++/OpenGL vector maps library with native SDKs for Android, iOS, Node.js, and OS X
- [Mapbox GL JS](https://github.com/mapbox/mapbox-gl-js) - JavaScript/WebGL vector maps library.
- [OpenLayers 3](https://github.com/openlayers/ol3/pull/4219) - JavaScript vector & raster library.
- [WhirlyGlobe/Maply](https://github.com/mousebird/WhirlyGlobe/blob/master/WhirlyGlobeSrc/WhirlyGlobe-MaplyComponent/src/MaplyMapnikVectorTiles.mm) - Objective C code that is able to read and render vector tiles(and style with mapnik xml) on iOS devices.
- [Leaflet.MapboxVectorTile](https://github.com/SpatialServer/Leaflet.MapboxVectorTile) is able to read PBF MapboxVectorTiles from a REST endpoint and render them as a TileLayer on a Leaflet Map. Use this option if you want to utilize vector tiles on a standard Leaflet web map without needing WebGL.
- [Nutiteq Maps SDK 3.x](https://developer.nutiteq.com) - C++ maps library for iOS, Android, Windows Phone and Xamarin with bindings for Java, ObjectiveC and C#
- [Mapzen Tangram](https://github.com/tangrams/tangram) - JavaScript library for rendering 2D & 3D maps live in a web browser with WebGL, supports MVT, GeoJSON, TopoJSON
- [Mapzen Tangram-es](https://github.com/tangrams/tangram-es) - C++ library for rendering 2D and 3D maps using OpenGL ES 2 with custom styling and interactions
* [mapbox-gl-leaflet](https://github.com/mapbox/mapbox-gl-leaflet) - Create Mapbox GL layers in Leaflet
* [react-native-mapbox-gl](https://github.com/mapbox/react-native-mapbox-gl) - Render Mapbox GL maps from React applications
* [hoverboard](https://github.com/devTristan/hoverboard) - Render vector tiles on canvas with Leaflet 0.7.x (supports GeoJSON, TopoJSON, and protobuf)
* [Leaflet.VectorGrid](https://github.com/IvanSanchez/Leaflet.VectorGrid) - Display gridded vector data (sliced GeoJSON, TopoJSON or Mapbox Vector Tiles) in Leaflet 1.0.0
* [ArcGIS API for JavaScript](https://developers.arcgis.com/javascript/) - Draw vector tile layers as part of your web map. Rendering done via `mapbox-gl-js` integration.
* [QMapboxGL](https://github.com/tmpsantos/qmapboxgl) – native vector maps library for Qt

### Applications / Command line tools

- [Mapbox Studio](https://github.com/mapbox/mapbox-studio) - Desktop design studio for both creating vector tiles from raw geodata and for rendering them on-the-fly into image tiles. Internally uses `tilelive.js` modules to handle vector tiles (see `tilelive-bridge` and `tilelive-vector`)
- [kosmtik](https://github.com/kosmtik/kosmtik) - Design maps with CartoCSS and Mapnik.
- [ArcGIS Pro](http://www.esri.com/en/software/arcgis-pro) - Generate vector tiles from maps authored in ArcGIS Pro or imported from ArcMap.

## CLI Utilities

- [Datamaps](https://github.com/ericfischer/datamaps) C application that can be used to create vector tiles and store them in an mbtiles. See the `render-vector` command.
- [tilemaker](https://github.com/systemed/tilemaker) - Command line tool to produce vector tiles directly from an .osm.pbf extract without an intermediate database.
- [vector-tiles-producer](https://github.com/vross/vector-tiles-producer) Command line tool in C++ to creates vector tiles for a given area at chosen zoom levels using a Mapnik XML.
- [tippecanoe](https://github.com/mapbox/tippecanoe) - Build vector tilesets from large collections of GeoJSON features.
- [vt-geojson](https://github.com/developmentseed/vt-geojson) - decodes vector tiles to GeoJSON FeatureCollections
- [tl](https://github.com/mojodna/tl) - An alternate command line interface to tilelive

## Mapbox GL JS Plugins

- [gl-draw](https://github.com/mapbox/gl-draw) - Adds support for drawing and editing features on Mapbox GL JS maps

## Servers

- [tessera](https://github.com/mojodna/tessera) - Supports serving and rendering vector tiles. Uses the same core libraries as Mapbox Studio.
- [tilestrata](https://github.com/naturalatlas/tilestrata) - with tilestrata-vt, can generate vector tiles
- [SpatialServer (PGRestAPI)](https://github.com/spatialdev/PGRestAPI) - A multi-purpose GeoSpatial NodeJS web server created at [SpatialDev](http://spatialdev.com) that not only serves MBTiles stuffed with vector tiles, it can also cut vector tiles on the fly from a PostGIS database.
- [Utilery](https://github.com/etalab/utilery) Server to generate vector tiles from PostGIS queries. Python based
- [Tilestache](https://github.com/mapzen/TileStache/) Mapzen fork. It supports mvt output tiles.
- [Kartotherian](https://github.com/kartotherian/kartotherian) Wikipedia tile server with [Tilerator](https://github.com/kartotherian/tilerator) backend tile pre-generator
- [ArcGIS Online](http://www.esri.com/software/arcgis/arcgisonline) - Supports serving vector tiles and rendering in the mapping application powered by the ArcGIS API for JavaScript
- [Portal for ArcGIS](http://www.esri.com/software/arcgis/arcgisserver/extensions/portal-for-arcgis) - Supports serving vector tiles and rendering in the mapping application powered by the ArcGIS API for JavaScript

## Low-level utilities

- [mapbox-gl-function](https://github.com/mapbox/mapbox-gl-function) - Mapbox GL style function evaluator
- [mapbox-gl-filter-simplify](https://github.com/mapbox/mapbox-gl-filter-simplify) - Simplifies and complexifies filters in Mapbox GL Styles
- [vt-pbf](https://github.com/anandthakker/vt-pbf) serialize JavaScript objects representing vector tiles into binary Protocol Buffer encodings of vector tiles

## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Tom MacWright](http://macwright.org) has waived all copyright and related or neighboring rights to this work.
