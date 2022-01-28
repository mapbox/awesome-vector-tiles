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
- [mapbox-vector-tile](https://github.com/mapzen/mapbox-vector-tile) is a Python package for vector tile encoding. Used in Mapzen's vector tile service [tileserver](https://github.com/tilezen/tileserver) and TileStache. [:warning:](https://github.com/tilezen/mapbox-vector-tile/issues/42) Only support V1 Tile spec and not V2, no longer maintained
- [geojson-vt](https://github.com/mapbox/geojson-vt) - Slice GeoJSON into vector tiles on the fly in the browser.
- [geojson2vt](https://github.com/geometalab/geojson2vt) - Python port of [geojson-vt](https://github.com/mapbox/geojson-vt) to convert GeoJSON into vector tiles.
- [java-vector-tile](https://github.com/ElectronicChartCentre/java-vector-tile) - A java encoder and decoder for vector tiles.
- [mapbox-vector-tile-java](https://github.com/wdtinc/mapbox-vector-tile-java) - Encode and decode v2.1 Mapbox Vector Tiles. Convert JTS Geometry to and from MVT features, including simple user data support. Utility functions for converting world coordinates to MVT coordinates and clipping to a tile envelope.
- [cached-vector-tile](https://github.com/developmentseed/cached-vector-tile) - An alternative implementation of the vector-tile-js interface, backed by plain JS objects/arrays rather than parsed-on-demand protobuf data. Trades away memory efficiency for faster feature.loadGeometry() calls.
- [tilegrinder](https://github.com/rastapasta/tilegrinder) - A helper library for applying a data altering function on each vector tile in an MBTiles, using the native protobuf wrapper for de- and encoding, recompressing the results and storing them either in an MBTiles or as single files.
- [SwiftVectorTiles](https://github.com/manimaul/SwiftVectorTiles) - A Swift encoder for vector tiles according to the Mapbox vector tile spec.
- [orb](https://github.com/paulmach/orb) - A Go geometry library with mvt <-> geojson support.
- [Charger](https://github.com/marauder-io/charger) - A Kotlin library providing vector tiles encoding, transformation and clipping functionalities.
- [dart-vector-tile](https://github.com/saigontek/dart-vector-tile) - A simple Dart package to encode & decode Mapbox Vector Tile.

## Clients

- [Mapbox GL Native](https://github.com/mapbox/mapbox-gl-native) - C++/OpenGL vector maps library with native SDKs for Android, iOS, Node.js, macOS, and Qt
- [Mapbox GL JS](https://github.com/mapbox/mapbox-gl-js) - JavaScript/WebGL vector maps library.
- [MapLibre GL](https://github.com/maplibre/maplibre-gl-js) - Is a community led fork derived from Mapbox GL JS prior to their switch to a non-OSS license.
- [OpenLayers](https://openlayers.org/en/latest/examples/mapbox-vector-layer.html) - JavaScript vector & raster library.
- [WhirlyGlobe/Maply](https://github.com/mousebird/WhirlyGlobe/tree/master/ios/library/WhirlyGlobe-MaplyComponent/src/vector_tiles/MaplyVectorTiles.mm) - Objective C code that is able to read and render vector tiles(and style with mapnik xml) on iOS devices.
- [Leaflet.MapboxVectorTile](https://github.com/SpatialServer/Leaflet.MapboxVectorTile) is able to read PBF MapboxVectorTiles from a REST endpoint and render them as a TileLayer on a Leaflet Map. Use this option if you want to utilize vector tiles on a standard Leaflet web map without needing WebGL.
- [CARTO Mobile SDK](https://github.com/CartoDB/mobile-sdk) - C++ maps library focused on offline features, for iOS, Android, Windows Phone and Xamarin with bindings for Java, Objective-C and C#. Based on [Nutiteq Maps SDK](https://developer.nutiteq.com), but open source and uses CartoCSS.
- [Mapzen Tangram](https://github.com/tangrams/tangram) - JavaScript library for rendering 2D & 3D maps live in a web browser with WebGL, supports MVT, GeoJSON, TopoJSON
- [Mapzen Tangram-es](https://github.com/tangrams/tangram-es) - C++ library for rendering 2D and 3D maps using OpenGL ES 2 with custom styling and interactions
* [mapbox-gl-leaflet](https://github.com/mapbox/mapbox-gl-leaflet) - Create Mapbox GL layers in Leaflet
* [react-native-mapbox-gl](https://github.com/mapbox/react-native-mapbox-gl) - Render Mapbox GL maps from React applications
* [hoverboard](https://github.com/devTristan/hoverboard) - Render vector tiles on canvas with Leaflet 0.7.x (supports GeoJSON, TopoJSON, and protobuf) [:warning:](https://github.com/madd512/hoverboard/issues/13#issuecomment-171406102) no longer maintained
* [Leaflet.VectorGrid](https://github.com/IvanSanchez/Leaflet.VectorGrid) - Display gridded vector data (sliced GeoJSON, TopoJSON or Mapbox Vector Tiles) in Leaflet 1.0.0
* [ArcGIS API for JavaScript](https://developers.arcgis.com/javascript/) - Draw vector tile layers as part of your web map. Rendering done via `mapbox-gl-js` integration.
* [mapscii](https://github.com/rastapasta/mapscii) - A Vector Tile to Braille and ASCII renderer for xterm-compatible terminals
* [Unofficial Mapbox GL Native bindings for Qt QML](https://github.com/rinigus/mapbox-gl-qml) - Qt QML bindings for Qt 5.6 and higher.
* [Mapbox-vector-tiles-basic-js-renderer](https://github.com/landtechnologies/Mapbox-vector-tiles-basic-js-renderer) - A fork of mapbox-gl-js giving you full control over rendering of specific tiles, also provides vector tile overlay for google maps.
* [QtPBFImagePlugin](https://github.com/tumic0/QtPBFImagePlugin) - Qt image plugin for displaying Mapbox vector tiles.
* [AliFlux VectorTileRenderer](https://github.com/AliFlux/VectorTileRenderer) - A highly customizable vector tile renderer built using C# for .Net platform. Comes with bindings for Mapsui and Gmap.Net components.
* [Azure Maps Web SDK](https://docs.microsoft.com/azure/azure-maps/) - Render vector tile layers on an interactive web map control using JavaScript or TypeScript.
* [Vector Tiles Google Maps](https://github.com/techjb/Vector-Tiles-Google-Maps) - Render vector tile layers on Google Maps.

### Applications / Command line tools

- [Mapbox Studio](https://www.mapbox.com/mapbox-studio/) - Web design studio for creating and styling vector tiles.
- [Mapbox Studio Classic](https://github.com/mapbox/mapbox-studio) - Desktop design studio for both creating vector tiles from raw geodata and for rendering them on-the-fly into image tiles. Internally uses `tilelive.js` modules to handle vector tiles (see `tilelive-bridge` and `tilelive-vector`) :warning: use [Mapbox Studio](https://www.mapbox.com/mapbox-studio/) instead.
- [kosmtik](https://github.com/kosmtik/kosmtik) - Design maps with CartoCSS and Mapnik.
- [ArcGIS Pro](http://www.esri.com/en/software/arcgis-pro) - Generate vector tiles from maps authored in ArcGIS Pro or imported from ArcMap.
- [MVT Styler](http://sputnik-maps.github.io/mvt-styler/) - map style editor for vector tiles.
- [Maputnik](https://github.com/maputnik/editor) - A visual style editor for the Mapbox GL style specification.
- [QGIS](https://qgis.org/) - supports vector tiles as a new map layer type since 3.14 release. It reads and displays styled vector tiles, adds styling GUI and writing (available as a processing toolbox algorithm).
- [QGIS Vector Tiles Reader](https://github.com/geometalab/Vector-Tiles-Reader-QGIS-Plugin) - QGIS Python plugin which reads Mapbox Vector Tiles from local MBTiles file or remote
- [mapbox-gl-inspect](https://github.com/lukasmartinelli/mapbox-gl-inspect) - Plugin for Mapbox GL JS to view the view and inspect VT features.
- [Mapbox MVT Chrome Extension](https://chrome.google.com/webstore/detail/mapbox-mvt/mfikcokdfehaofebfhoehbajfgbofdpk) - Google Chrome extension that parses loaded vector tiles on the fly, shows short statistics and shows each vector tile as GeoJSON
- [Fresco](https://github.com/go-spatial/fresco) - is an open source Mapbox Vector Tile Style editor.
- [Baremaps](https://www.baremaps.com/) - An open source pipeline for producing Mapbox vector tiles from OpenStreetMap with Postgis and Java.

## CLI Utilities

- [mbview](https://github.com/mapbox/mbview) - Watch MBTiles in your localhost. View tiles in a basic Mapbox GL JS webapp locally
- [tippecanoe](https://github.com/mapbox/tippecanoe) - Build vector tilesets from large collections of GeoJSON features.
- [tilemaker](https://github.com/systemed/tilemaker) - Command line tool to produce vector tiles directly from an .osm.pbf extract without an intermediate database.
- [mapbox-filter](https://github.com/ondrap/mapbox-filter) - Filter MBTiles according to Mapbox GL JS styles, shrink MBTiles directly, serve locally over http, publish to S3-compatibile storage
- [vector-tiles-producer](https://github.com/vross/vector-tiles-producer) Command line tool in C++ to creates vector tiles for a given area at chosen zoom levels using a Mapnik XML. :warning: no longer maintained
- [vt-geojson](https://github.com/developmentseed/vt-geojson) - decodes vector tiles to GeoJSON FeatureCollections
- [tl](https://github.com/mojodna/tl) - An alternate command line interface to tilelive
- [tileshrink](https://github.com/rastapasta/tileshrink) - Reduce the layer extent and simplify the resulting geometries of all vector tiles in an MBTiles
- [tiler @GeoVation](https://github.com/Geovation/tiler) - Command line tool for converting GeoJSON, Shapefiles or PostGIS layer to raw Vector Tiles (or MBTiles)
- [tiler @thomersch](https://github.com/thomersch/grandine/tree/master/cmd/tiler) - Command line tool to convert GeoJSON to Vector Tiles (written in Go language).
- [geojson2mvt](https://github.com/NYCPlanning/geojson2mvt) - npm package for building a static vector tile tree for given xyz bounds from a geojson file (uses [geojson-vt](https://github.com/mapbox/geojson-vt))
- [OGR MVT](http://gdal.org/drv_mvt.html) and [MBTiles](http://gdal.org/frmt_mbtiles.html) - The GDAL/OGR MVT and MBTILES drivers can be used to read and write vector tiles, respectively as tileset on the filesystem or in a mbtiles container (GDAL >= 2.3.0)
- [MBUtil](https://github.com/mapbox/mbutil) - Import and export MBTiles to disk :warning: no longer maintained
- [Datamaps](https://github.com/ericfischer/datamaps) C application that can be used to create vector tiles and store them in an mbtiles. See the `render-vector` command. :warning: no longer maintained, use tippecanoe instead
- [vt2geojson](https://github.com/wangyoucao577/vt2geojson) Command line tool to convert Vector Tiles to GeoJSON (written in `Go` language based on the awesome [orb](https://github.com/paulmach/orb) package).
- [python-vt2geojson](https://github.com/Amyantis/python-vt2geojson) - Command line tool and Python package for converting vector tiles into GeoJSON.
- [vt2geojson](https://github.com/mapbox/vt2geojson) - Command line tool and npm package for converting vector tiles into GeoJSON.
- [tileinfo](https://www.npmjs.com/package/tileinfo) - Display TileJSON info about an mbtiles file.
- [XYZ](https://github.com/dechristopher/xyz) - Simple tool to procedurally prime XYZ tile caches to a given zoom level.
- [Planetiler](https://github.com/onthegomap/planetiler) - Command-line Java program to build planet-scale vector tilesets from OpenStreetMap data in a few hours.

## Mapbox GL JS Plugins

- [gl-draw](https://github.com/mapbox/gl-draw) - Adds support for drawing and editing features on Mapbox GL JS maps

## Servers

- [ArcGIS Online](http://www.esri.com/software/arcgis/arcgisonline) - Supports serving vector tiles and rendering in the mapping application powered by the ArcGIS API for JavaScript
- [Cloud-Tileserver](https://github.com/henrythasler/cloud-tileserver) - Serve vector tiles with AWS. Includes a Lambda-Function written in Typescript to dynamically create vector tiles with postgis. Terraform configuration and step-by-step tutorial is also included.
- [ClusterBuster](https://github.com/chargetrip/clusterbuster) A Mapbox Vector Tile (MVT) map tiling server with built-in clustering and filtering.
- [djangorestframework-mvt](https://github.com/corteva/djangorestframework-mvt) - A Django REST Framework extension for creating views that serve Postgres data as tiles.  Tiles can be paginated and filtered by their properties.
- [GeoServer](http://geoserver.org) - java web application for sharing and editing geospatial data. [Vector tile extension](https://docs.geoserver.org/latest/en/user/extensions/vectortiles/index.html) available since GeoServer 2.11.
- [go-vtile-example](https://github.com/vicapow/go-vtile-example) - An example server written in Go
- [Hastile](https://github.com/indicatrix/hastile) - Haskell web server using PostGIS to deliver vector tiles.
- [Kartotherian](https://github.com/kartotherian/kartotherian) Wikipedia tile server with [Tilerator](https://github.com/kartotherian/tilerator) backend tile pre-generator
- [LOD](https://github.com/tile-fund/lod) - A thin map tile proxy with in-memory caching and a slim authentication backend.
- [MapServer](https://mapserver.org/) - Open Source platform, written in C, for publishing spatial data and interactive mapping applications to the web. MVT output available since version 7.2
- [martin](https://github.com/urbica/martin) - is a PostGIS vector tiles server suitable for large databases.
- [mbtileserver](https://github.com/consbio/mbtileserver) - A simple Go-based server for map tiles stored in mbtiles format.
- [OpenMapTiles](https://github.com/openmaptiles) - Set of open-source tools for self-hosting of OpenStreetMap maps in more than 50 languages. It provides both raster as well as vector tiles, WMS and WMTS services for GIS programs, support for JavaScript viewers and mobile SDK.
- [OSM Scout Server](https://rinigus.github.io/osmscout-server/) - Maps server providing vector and raster tiles, geocoder, and router. Designed to be used on Linux (mobile and PC) to provide offline maps; written in C++
- [Portal for ArcGIS](http://www.esri.com/software/arcgis/arcgisserver/extensions/portal-for-arcgis) - Supports serving vector tiles and rendering in the mapping application powered by the ArcGIS API for JavaScript
- [postserve](https://github.com/openmaptiles/postserve) - A small Python based tileserver using ST_AsMVT and ST_AsMVTGeom to generate vector tiles on the fly. Designed for use with PostGIS 2.4 and the OpenMapTiles project
- [t-rex](https://github.com/pka/t-rex/) - MVT server in a single executable written in Rust. Serves tiles from PostGIS supporting custom tile grids.
- [Tegola](https://github.com/go-spatial/tegola) - is a vector tile server delivering Mapbox Vector Tiles with support for PostGIS and GeoPackage data providers.
- [tessella](https://github.com/urbica/tessella) - lightweight Node.js Mapbox Vector Tiles server. Inspired by tessera.
- [tessera](https://github.com/mojodna/tessera) - Supports serving and rendering vector tiles. Uses the same core libraries as Mapbox Studio.
- [tileserver](https://github.com/tilezen/tileserver) Mapzen Vector Tile Service.
- [tileserver-gl](https://github.com/maptiler/tileserver-gl) Vector and raster maps with GL styles. Server side rendering by Mapbox GL Native. Map tile server for Mapbox GL JS, Android, iOS, Leaflet, OpenLayers, GIS via WMTS, etc.
- [tilesplash](https://github.com/faradayio/tilesplash) - A light and quick nodejs webserver for serving topojson or mapbox vector tiles from a postgis backend
- [TileStache](https://github.com/TileStache/TileStache) added support for Mapbox Vector tiles via .pbf extension requests.
- [tilestrata](https://github.com/naturalatlas/tilestrata) - with tilestrata-vt, it can generate Mapnik Vector Tiles; with [tilestrata-postgismvt](https://github.com/Stezii/tilestrata-postgismvt), it can serve Mapbox Vector Tiles from a PostGIS db
- [Tyler](https://github.com/marauder-io/tyler) - An Open Source tiling server maintaining a Vector Tile storage providing a REST interface.
- [SpatialServer (PGRestAPI)](https://github.com/spatialdev/PGRestAPI) - A multi-purpose GeoSpatial NodeJS web server created at [SpatialDev](http://spatialdev.com) that not only serves MBTiles stuffed with vector tiles, it can also cut vector tiles on the fly from a PostGIS database. [:warning:](https://github.com/spatialdev/PGRestAPI/issues/142#issuecomment-231132808) No longer maintained.
- [Utilery](https://github.com/etalab/utilery) Server to generate vector tiles from PostGIS queries. Python based [:warning:](https://github.com/tilery/utilery/issues/6) no longer maintained.
- [pg_tileserv](https://github.com/CrunchyData/pg_tileserv) - A very thin PostGIS-only tile server in Go. Takes in HTTP tile requests, executes SQL, returns MVT tiles.
- [ngx_http_mbtiles_module](https://github.com/durkie/ngx_http_mbtiles_module) - Serve mbtiles files directly from nginx. Ideal for low-resource environments or situations where the mbtiles contents are changing frequently.
- [TiMVT](https://github.com/developmentseed/timvt) - A lightweight PostGIS based dynamic vector tile server.
- [Vallaris Maps](https://vallarismaps.com) - Mapping Platforms to storage process and services GIS Data. Provide DataService API and Maps API (Vector Tiles, WMS, WMTS) Compilance in OGC API Standards.

## Low-level utilities

- [vt-pbf](https://github.com/anandthakker/vt-pbf) serialize JavaScript objects representing vector tiles into binary Protocol Buffer encodings of vector tiles
- [vtzero](https://github.com/mapbox/vtzero) - minimalist vector tile decoder and encoder in C++
- [mvt-fixtures](https://github.com/mapbox/mvt-fixtures/) - a suite of valid and invalid test fixtures according to the Mapbox Vector Tile spec versions. Includes simplified unit test fixtures and real-world fixtures to test your encoders and decoders.
- [zellige](https://github.com/sitewisely/zellige) - command line utility written to convert GeoJSON to MVT.
- [mapbox-gl-function](https://github.com/mapbox/mapbox-gl-function) - Mapbox GL style function evaluator :warning: now maintained as party of mapbox-gl-js
- [mapbox-gl-filter-simplify](https://github.com/mapbox/mapbox-gl-filter-simplify) - Simplifies and complexifies filters in Mapbox GL Styles :warning: removed

## Articles

- [Vector tiles remixed](http://gdunlop.github.io/Vector-tiles-remixed/) - guide to using [tilemaker](https://github.com/systemed/tilemaker) to generating vector tiles
- [Build Your Own Static Vector Tile Pipeline](https://geovation.github.io/build-your-own-static-vector-tile-pipeline) - guide transforming, encoding and hosting tiles in the cloud; using ogr2ogr + tippecanoe + Mapbox GL JS
- [Using the new MVT function in PostGIS](https://medium.com/nycplanninglabs/using-the-new-mvt-function-in-postgis-75f8addc1d68) - Building a vector tile service with PostGIS, express, and pg-promise.
- [Serverless Vector Tiles on AWS](https://github.com/addresscloud/serverless-tiles)
- [Tegola OSM/OMT Import Procedure](https://github.com/dechristopher/tegola-omt) - This document outlines everything necessary to build, from scratch, an operational OpenStreetMap vector tile server. The stack consists of the latest LTS Ubuntu Server distribution, Tegola as the tile server, PostgreSQL as the database, and the use of the open source OpenMapTiles standard schema.

## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Tom MacWright](http://macwright.org) has waived all copyright and related or neighboring rights to this work.
