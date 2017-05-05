### Table of Contents

- [GTFS](#gtfs)
  - [GTFS Libraries](#gtfs-libraries)
  - [GTFS Tools](#gtfs-tools)
  - [GTFS Validators](#gtfs-validators)
- [GTFS Realtime](#gtfs-realtime)
  - [GTFS Realtime Libraries & Demo Apps](#gtfs-realtime-libraries--demo-apps)
  - [GTFS Realtime Validators](#gtfs-realtime-validators)
  - [GTFS Realtime Archival Tools](#gtfs-realtime-archival-tools)
  - [GTFS Realtime Convertors](#gtfs-realtime-convertors)
  - [GTFS Realtime Utilities](#gtfs-realtime-utilities)
- [SIRI](#siri)
- [Data](#data)
- [APIs](#apis)
- [Resources](#resources)
- [Visualizations](#visualizations)


### GTFS

- [GTFS Spec](https://developers.google.com/transit/gtfs/) - Specification for the General Transit Data Feed, or GTFS.
- [GTFS Best Practices](http://gtfs.org/best-practices/) - Best practices for producers of a GTFS feed.

#### GTFS Libraries

Software that makes it easy to consume GTFS data in a variety of languages.

- [Mapzen GTFS](https://github.com/transitland/mapzen-gtfs) - A Python GTFS library that supports reading individual GTFS tables, or constructing a graph to represent each agency in a feed.
- [gtfsdb](https://github.com/OpenTransitTools/gtfsdb) - Python library for converting GTFS files into a relational database.
- [OneBusAway GTFS Modules](https://github.com/OneBusAway/onebusaway-gtfs-modules/wiki) - A Java-based library for reading, writing, and transforming public transit data in the GTFS format, including database support.
- [GTFS to SQL](https://github.com/TransitFeeds/GtfsToSql) - Parses a GTFS feed into an SQL database (used in [TransitFeeds.com](http://transitfeeds.com/))
- [SQL to GTFS](https://github.com/TransitFeeds/SqlToGtfs) - Convert an SQLite file generated with "GtfsToSql" back to a zipped GTFS file.
- [Go GTFS Parser](https://github.com/geops/gtfsparser) - A GTFS parsing library for Go
- [GTFS Feed Parser](https://github.com/OsmSharp/GTFS) - .Net/Mono implementation of a GTFS parser
- [Node-GTFS](https://github.com/brendannee/node-gtfs) - Loads transit data from [GTFS Data Exchange](http://www.gtfs-data-exchange.com/), unzips it and stores it to a MongoDB database and provides some methods to query for agencies, routes, stops and times.
- [GTFS-viz](https://github.com/vasile/GTFS-viz) - Ruby script that converts a set of GTFS files into a SQLite database + GeoJSONs (needed by the [Transit Map](https://github.com/vasile/transit-map) web application)
- [GTFS-OSM-Sync](https://github.com/CUTR-at-USF/gtfs-osm-sync) - A Java tool for syncrhonizing data in GTFS format with [OpenStreetMap.org](http://www.openstreetmap.org/).
- [gtfs-sequelize](https://github.com/evansiroky/gtfs-sequelize) - Node.js library modeling the static GTFS using [sequelize.js](http://sequelizejs.com/).
- [gtfslib-python](https://github.com/afimb/gtfslib-python) -  An open source library in python for reading GTFS files and computing various stats and indicators about Public Transport networks.
- [multigtfs](https://github.com/tulsawebdevs/django-multi-gtfs) - A Django application to import and export GTFS
- [GTFSTK](https://github.com/araichev/gtfstk) - A Python 3 toolkit for analyzing GTFS data in memory. Uses Pandas and Shapely for speed.

#### GTFS Converters

Converters from various static schedule formats to GTFS. 

- [Transmodel and IFF to GTFS](https://github.com/bliksemlabs/bliksemintegration) - Imports and syncs (Transmodel) BISON Koppelvlak1, IFF (a format written by HP/EDS, somewhat similiar to ATCO CIF) to import timetables of the railway networks. The internal pseudo-NETeX datastructure allows to export to GTFS and there are proof-of-concepts to export to other formats such as NETeX, GTFS and IFF.
- [Open-Transport SYNTHESE Convertors](https://github.com/Open-Transport/synthese/wiki) - Converts French-Transmodel, SIRI, NETeX, HAFAS, HASTUS, VDV452, and more.
- [Chouette](http://www.chouette.mobi/) - Converts French-Transmodel, SIRI, NETeX. See Chouette.mobi website for more info.
 
#### GTFS Tools

- [bus-router](https://github.com/atlregional/bus-router) - Python script that generates missing shapes.txt for GTFS using routing from [Google Maps Directions API](https://developers.google.com/maps/documentation/directions/) or [OSRM](https://github.com/Project-OSRM/osrm-backend/wiki/Server-api).
- [GTFS Editor](https://github.com/conveyal/gtfs-editor) A (self-hosted) web-based GTFS editing framework.
- [GTFS Editor for Vagrant](https://github.com/laidig/vagrant-gtfs-editor) Quickly set up the GTFS editor (above) using [Vagrant](https://www.vagrantup.com/)
- [TransitWand](http://transitwand.com/) - An open source web and mobile application for collecting transit data. Use it to create GTFS feeds, capture passenger counts or generate GIS datasets.
- [Gtfs Data Manager](https://github.com/conveyal/gtfs-data-manager) - A workflow tool for managing large amounts of GTFS data and importing them into OpenTripPlanner.

 
#### GTFS Validators

- [feedValidator](https://github.com/google/transitfeed/wiki/FeedValidator) - Google supported Python-based GTFS validator. 
- [gtfs-validator](https://github.com/conveyal/gtfs-validator) - - A GTFS validator based on the OneBusAway GTFS Modules, runs in Java and is faster than the Google provided one. 
- [GFTS Data Package Specification](https://github.com/Stephen-Gates/GTFS) - A [Data Package specification](http://specs.frictionlessdata.io/data-packages/) with validation accomplished with [Good Tables](http://goodtables.okfnlabs.org/). Includes a data package, schemas, tests, and uses South East Queensland GTFS data as an example.
- [GTFS Meta-Validator](http://gtfsvalidator.omnimodal.io) - A web-based GTFS validator that runs both [feedValidator](https://github.com/google/transitfeed/wiki/FeedValidator) and [gtfs-validator](https://github.com/conveyal/gtfs-validator) on uploaded GTFS files.

### GTFS Realtime

#### GTFS Realtime Libraries & Demo Apps

- [gtfs-realtime-bindings](https://github.com/google/gtfs-realtime-bindings) - The official bindings for Java, .NET, Node.js, Python, and Ruby generated from the official [GTFS-realtime protocol buffer specification](https://github.com/google/transit/blob/master/gtfs-realtime/proto/gtfs-realtime.proto).
- [GTFS-realtime Exporter](https://github.com/OneBusAway/onebusaway-gtfs-realtime-exporter/wiki) - A Java-based tool that assists in producing and sharing a GTFS-relatime feed.
- [GTFS-realtime Alerts Producer Demo](https://github.com/OneBusAway/onebusaway-gtfs-realtime-alerts-producer-demo/wiki) - A Java-based demo project for producing GTFS-realtime Service Alerts.
- [GTFS-realtime Alerts Producer Web Application](https://github.com/OneBusAway/onebusaway-service-alerts) - A Java-based web application for producing GTFS-realtime Service Alerts.
- [GTFS-realtime TripUpdates & VehiclePositions Producer Demo](https://github.com/OneBusAway/onebusaway-gtfs-realtime-trip-updates-producer-demo/wiki) - A Java-based demo project for producing GTFS-realtime TripUpdates (estimated arrivals) and Vehicle Positions.
- [GTFS-realtime Vehicle Positions Consumer/Visualizer Demo](https://github.com/OneBusAway/onebusaway-gtfs-realtime-visualizer/wiki) - A Java-based demo project for consuming a GTFS-realtime Vehicle Positions feed and displaying this info on a map.

#### GTFS Realtime Validators

- [gtfs-realtime-validator](https://github.com/CUTR-at-USF/gtfs-realtime-validator) - A GTFS-realtime validation tool developed by the Center for Urban Transportation Research at the University of South Florida.  Also includes an integrated version of the [gtfs-validator](https://github.com/conveyal/gtfs-validator) tool.

#### GTFS Realtime Archival Tools

- [GTFS-realtime to SQL](https://github.com/TransitFeeds/GtfsRealTimeToSql) - Parses a GTFS-RealTime feed into an SQL database (used in [TransitFeeds.com](http://transitfeeds.com/))
- [gtfsrdb](https://github.com/CUTR-at-USF/gtfsrdb) - A Python tool that supports reading and archiving GTFS-realtime feeds into a database

#### GTFS Realtime Convertors

- [SIRI to GTFS-realtime](https://github.com/OneBusAway/onebusaway-gtfs-realtime-from-siri-cli/wiki) - A Java-based command-line utility to convert from the [SIRI format](http://user47094.vs.easily.co.uk/siri/) to GTFS-realtime
- [OrbCAD SQL Server to GTFS-realtime](https://github.com/CUTR-at-USF/HART-GTFS-realtimeGenerator/wiki) - A Java-based command-line utility that extracts vehicle positions and trip updates information from an OrbCAD SQL Server and exports them to the GTFS-realtime TripUpdates and VehiclePositions formats.
- [NextBus API to GTFS-realtime](https://github.com/OneBusAway/onebusaway-gtfs-realtime-from-nextbus-cli/wiki) - A Java-based command-line utility to convert from the [NextBus API format](http://www.nextbus.com/xmlFeedDocs/NextBusXMLFeed.pdf) to GTFS-realtime.  Note that NextBus now directly offers a GTFS-realtime API for their products.  See [Cubic site](http://nextbus.cubic.com/Products/Real-Time-Rider-Information) and [this FAQ](https://medium.com/omnimodal/want-more-riders-open-up-your-nextbus-api-with-gtfs-realtime-7387c80f31e1#.pkuzizhl5).
- [Syncromatics API to GTFS-realtime](https://github.com/CUTR-at-USF/bullrunner-gtfs-realtime-generator) - A Java-based command-line utility to convert from the [Syncromatics API](http://www.syncromatics.com/) format to GTFS-realtime TripUpdates and VehiclePositons.
- [KV6,15,17, and ARNU to GTFS-realtime](https://github.com/bliksemlabs/bliksemintegration-realtime) - Java-based tool to process incoming KV6,15,17 and ARNU and match them to static transit data present in a RID integration database. It then proceeds to export this data as ARNU RITinfo, GTFS(realtime) and KV78turbo
- [WMATA BusPositions API to GTFS-realtime](https://github.com/kurtraschke/wmata-gtfsrealtime) - Java-based tool to convert from WMATA's [BusPositions API](https://developer.wmata.com/docs/services/54763629281d83086473f231/operations/5476362a281d830c946a3d68) and Alert RSS feeds from [MetroAlerts](http://www.wmata.com/rider_tools/metro_service_status/rail_bus.cfm?) to GTFS-realtime TripUpdates, VehiclePositions, and Alerts feeds.
- [SEPTA API to GTFS-realtime](https://github.com/kurtraschke/septa-gtfsrealtime) - Java-based tool to convert [SEPTA's](http://www.septa.org/) [real-time bus and rail data](http://www3.septa.org/hackathon/) to GTFS-realtime
- [CTA API to GTFS-realtime](https://github.com/kurtraschke/ctatt-gtfsrealtime) - Java-based tool to convert [CTA's](http://www.transitchicago.com/) [Train Tracker data](http://www.transitchicago.com/developers/traintracker.aspx) to GTFS-realtime.
- [Detroit DOT to GTFS-realtime](https://github.com/prashtx/ddot-avl) - Extract real-time info from [DDOT's](http://www.detroitmi.gov/How-Do-I/Locate-Transportation/Bus-Schedules) TransitMaster installation (database) and convert to GTFS-realtime
- [Live Transit Event Trigger](https://github.com/ipublic/live_transit_event_trigger) - Extracts data from [Ride On's](http://www.montgomerycountymd.gov/dot-transit/) OrbCAD database and export as GTFS-realtime.
- [SoundTransit to GTFS-realtime](https://github.com/bdferris/onebusaway-sound-transit-realtime) - Convert text file feed from [Sound Transit](http://www.soundtransit.org/) to GTFS-realtime
- [Civic Transit](https://github.com/jestin/CivicTransit) - Screen-scrapes [KCATA’s](http://www.kcata.org/) TransitMaster WebWatch installation to produce a GTFS-realtime feed.

#### GTFS Realtime Utilities

- [gtfs-rt-dump](https://github.com/kurtraschke/gtfs-rt-dump) - Converts protocol buffer format to plain text for easy viewing of a GTFS-realtime feed in plain text (for debugging purposes)
- [GTFS-realtime Munin Plugin](https://github.com/OneBusAway/onebusaway-gtfs-realtime-munin-plugin) - Provides a [Munin](http://munin-monitoring.org/) plugin for logging information about a GTFS-realtime feed.
- [GTFS-realtime Nagio Plugin](https://github.com/OneBusAway/onebusaway-gtfs-realtime-nagios-plugin) - Provides a [Nagios](https://www.nagios.org/) plugin for monitoring a GTFS-realtime feed
- [GTFS-realtime-test-service](https://github.com/CUTR-at-USF/gtfs-realtime-test-service) - A tool for mocking GTFS-realtime feed content (e.g., for use in testing a GTFS-realtime consuming application)


### SIRI

- [SIRI API](https://github.com/OneBusAway/onebusaway/wiki/SIRI-Resources) - Java classes generated from the v1.0 and v1.3 [SIRI](http://user47094.vs.easily.co.uk/siri/) schemas.
- [SIRI 2.0 API](https://github.com/laidig/siri-20-java) - Java classes generated from the v2.0 [SIRI](http://user47094.vs.easily.co.uk/siri/) schemas.
- [SIRI to GTFS-realtime](https://github.com/OneBusAway/onebusaway-gtfs-realtime-from-siri-cli/wiki) - A Java-based command-line utility to convert from the [SIRI format](http://user47094.vs.easily.co.uk/siri/) to GTFS-realtime.
- [SIRI 2.0 Autodoc](https://laidig.github.io/siri-20-java/doc/) - Automatically generated documentation from the (incredibly well) annotated SIRI 2.0 Schema Definition. 
- [King County Metro Legacy AVL to SIRI](https://github.com/bdferris/onebusaway-king-county-metro/tree/master/onebusaway-king-county-metro-legacy-avl-to-siri) - Java-based tool to convert [King County Metro's](http://metro.kingcounty.gov/) Legacy AVL format to SIRI.
- [SIRI REST Client](https://github.com/CUTR-at-USF/SiriRestClient/wiki) - An open-source Android library for interacting with the RESTful SIRI interface for real-time transit data, such as that currently being used by the [MTA Bus Time API](http://bustime.mta.info/wiki/Developers/SIRIIntro).
- [SIRI 1.3 POJOs (Android-compatible)](https://github.com/CUTR-at-USF/onebusaway-siri-api-v13-pojos/wiki) - Android-compatible Plain Old Java Objects (POJOSs) used for data binding (deserliazing XML/JSON) responses for SIRI v1.3 APIs.  Used by the [SIRI REST Client](https://github.com/CUTR-at-USF/SiriRestClient/wiki).

### Data

- [Transitland](https://transit.land/) - Community editable list of many transit agency GTFS datasets. Also provides an API to access the data as JSON/GeoJSON and a playground to try out the data.
- [National Transit Database](http://www.ntdprogram.gov/) - Information and statistics on the transit systems of the United States, run by the Federal Transit Administration.
- [TransitFeeds](http://transitfeeds.com/) - List of GTFS and GTFS-RT feeds. [Archives and validates](http://transitfeeds.com/p/capital-metro/24) the GTFS feeds and allows you to preview both [GTFS](http://transitfeeds.com/p/capital-metro/24/20151015) and [GTFS-RT](http://transitfeeds.com/p/capital-metro/495) through the browser. 
- [GTFS Data Exchange](http://www.gtfs-data-exchange.com/agencies) - Used to be the definitive list of GTFS links. Shutdown in 2016. But 93G of data from 2008 to 2016 is available upon request.

## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, Luqmaan Dawoodjee has waived all copyright and related or neighboring rights to this work.
