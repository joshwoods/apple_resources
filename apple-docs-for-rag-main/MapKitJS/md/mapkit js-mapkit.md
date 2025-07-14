

- MapKit JS
-  mapkit 

Class

# mapkit

The JavaScript API for embedding Apple Maps on your website.

MapKit JS 5.0+

``` source
interface mapkit
```

## Mentioned in 

Creating a Maps token

## Overview

The mapkit object is the main namespace for the MapKit JS framework. Similar to MapKit for apps, you can use MapKit JS to display interactive maps with customized annotations and overlays, and provide directions and search services. Your app can supply step-by-step navigation, and help a user find a location by autocompleting a search query.

MapKit JS lets you customize the look of your map. You can choose style details for overlays and annotations, display a standard street map or one that uses satellite imagery, and adjust the visibility of map controls. Additionally, you can customize a map’s behavior by providing event handlers that cause the map to scroll or respond when users select items. You can also enable or disable panning, zooming, and rotation.

## Topics

### Initialization

Handling initialization events

Respond to events that trigger when MapKit JS initializes.

init

Initializes MapKit JS by providing an authorization callback function and optional language.

MapKitInitOptions

Initialization options for MapKit JS.

Libraries

The list of available libraries.

loadedLibraries

A string that describes the list of loaded libraries.

load

Tells MapKit JS which libraries to load.

addEventListener

Subscribes a listener function to an event type.

removeEventListener

Unsubscribes a listener function from an event type.

### Maps

mapkit.Map

An embeddable interactive map that you add to a webpage.

maps

An array that automatically adds and removes maps as the framework creates and destroys them.

### Annotations and overlays

Annotations

Create annotations to add indicators and additional details for specific locations on a map.

Overlays

Create overlays to highlight geographic regions or paths.

### Geocoder

mapkit.Geocoder

A geocoder that converts human-readable addresses to geographic coordinates, and vice versa.

### Search

mapkit.AddressCategory

The categories of address components that users can search for with an address filter.

mapkit.AddressFilter

An object that filters which address options to include or exclude in search results.

mapkit.Search

An object that retrieves map-based search results for a user-entered query.

### Points of interest

mapkit.filterExcludingAllCategories

A value that excludes all point-of-interest categories.

mapkit.filterIncludingAllCategories

A value that includes all point-of-interest categories.

mapkit.PointOfInterestFilter

A filter for determining the points of interest to include or exclude on a map or in a local search.

mapkit.PointsOfInterestSearch

An object that fetches points of interest within a specified region.

mapkit.MapFeatureAnnotation

An object that represents a map feature that the user selects.

mapkit.MapFeatureAnnotationGlyphImage

An object that describes map feature annotation images.

mapkit.PointOfInterestCategory

Point-of-interest categories.

mapkit.MapFeatureType

Values that describe the feature type of a point of interest.

### Directions

mapkit.Directions

An object that provides directions and estimated travel time based on the options you provide.

### Map view customization

mapkit.Padding

The values that define content padding within the map view frame.

mapkit.FeatureVisibility

Constants indicating the visibility of different adaptive map features.

### Geographical features

importGeoJSON

Converts imported GeoJSON data to MapKit JS items.

GeoJSONDelegate

A delegate object that controls a GeoJSON import to override default behavior and provide custom style.

ItemCollection

A tree structure containing annotations, overlays, and nested item collection objects.

Displaying Indoor Maps with MapKit JS

Use the Indoor Mapping Data Format (IMDF) to show an indoor map with custom overlays and points of interest in your browser.

### Places

Place

A place object that returns from a geocoder lookup, a reverse lookup, or a fetch request for points of interest.

PlaceDetailOptions

mapkit.PlaceLookup

An object that provides the ability to look up place information for a specified Place ID.

placeDetails

A list of all user-created place detail objects that are currently active on a page.

PlaceLookupOptions

The options for creating a place lookup.

PlaceSelectionAccessoryOptions

The options for selection accessories.

mapkit.PlaceAnnotation

An annotation for a place.

mapkit.PlaceDetail

An interactive view that displays information about a place.

mapkit.PlaceSelectionAccessory

The accessory that conveys information about a place associated with an annotation.

### Map coordinates

mapkit.Coordinate

An object representing the latitude and longitude for a point on the Earth’s surface.

mapkit.CoordinateRegion

A rectangular area on a map that a center coordinate and a span define, in degrees of latitude and longitude.

mapkit.CoordinateSpan

The width and height of a map region.

mapkit.BoundingRegion

A rectangular area on a map, which coordinates of the rectangle’s northeast and southwest corners define.

### Map units

mapkit.MapPoint

A location, in map units, of a point on the Earth’s surface projected onto a 2D map.

mapkit.MapRect

A rectangular region, in map units, of a two-dimensional map projection.

mapkit.MapSize

A pair of values, in map units, that define the width and height of a rectangular area of a map projection.

mapkit.CameraZoomRange

A minimum and maximum camera distance, in meters, from the center of the map.

### Version and language

language

A language ID indicating the selected language.

build

The build string.

version

The version of MapKit JS.

### Response objects

FetchResponse

An object that contains data MapKit JS returns from a place search request.

### Delegates

FetchDelegate

An object to pass to a map feature annotation to fetch place objects instead of a callback function.

ImageDelegate

An object you use to specify image URLs.

## See Also

### Essentials

Displaying place information using the Maps Embed API

Show place information on a map using a URL.

Creating a Maps token

Generate your token to access MapKit services with proper authorization.

Loading the latest version of MapKit JS

Link to the most recent autoupdating version of MapKit JS, or a version of your choice.

