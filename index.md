# HCTG GTFS Workshop

## Useful links

- [GTFS Reference](https://gtfs.org/documentation/schedule/reference/)
- [Transitland Global Transit Map](https://www.transit.land/map)
- [Leaflet Quick Start Guide](https://leafletjs.com/examples/quick-start/)

## Tutorial Files

Download GTFS files for your local transit system (a good directory of transit feeds is Transitland, linked above) and place them in `gtfs/`, replacing the files currently in it if applicable. The following are tutorial files which show the process of building a Leaflet map with GTFS data step-by-step:

- [step-1.html](./step-1.html)
- [step-2.html](./step-2.html)
- [step-3.html](./step-3.html)
- [step-4.html](./step-4.html)
- [step-5.html](./step-5.html)
- [step-6.html](./step-6.html)

## Potential Next Steps

- Show overlapping transit routes in some way? (the current popup only shows the route on the "top-most layer" of the map, i.e. the one which was added last to the map)
- Plot stops/stations on the map?
  - Read the documentation for [stops.txt](https://gtfs.org/documentation/schedule/reference/#stopstxt)
  - There will be a large number of stops which may overcrowd the map. Hint: the tutorial files already include [something](https://github.com/Leaflet/Leaflet.markercluster) which may solve this problem :)
- Display schedules for routes and/or stops?
  - Read the documentation for [stop_times.txt](https://gtfs.org/documentation/schedule/reference/#stop_timestxt)
- ADVANCED: Integrate with your transit service's API or GTFS-RT feed to show real-time vehicle locations and estimated arrival times?
  - [GTFS Realtime documentation](https://gtfs.org/documentation/realtime/reference/)
  - Almost all transit agencies with their own "live map" use JSON APIs to fetch vehicle locations and estimated arrival times. Find these APIs using your browser's network inspector and try to integrate them into your map!