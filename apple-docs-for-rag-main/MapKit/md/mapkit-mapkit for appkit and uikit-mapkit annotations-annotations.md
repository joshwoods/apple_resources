

- MapKit
- MapKit for AppKit and UIKit
-  MapKit annotations 

API Collection

# MapKit annotations

Create annotations to add indicators and additional details for specific locations on a map.

## Topics

### Location annotations

Annotating a Map with Custom Data

Annotate a map with location-specific data using default and customized annotation views and callouts.

class MKPointAnnotation

A string-based piece of location-specific data that you apply to a specific point on a map.

class MKMapItemAnnotation

An annotation that represents a map item

class MKMarkerAnnotationView

An annotation view that displays a balloon-shaped marker at the designated location.

class MKPinAnnotationView

An annotation view that displays a pin image on the map.

Deprecated

### Grouped annotations

Decluttering a Map with MapKit Annotation Clustering

Enhance the readability of a map by replacing overlapping annotations with a clustering annotation view.

class MKClusterAnnotation

An annotation that groups two or more distinct annotations into a single entity.

### User location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

class MKUserLocation

An annotation that reflects the user’s location on the map.

class MKUserLocationView

A configurable annotation that shows the user’s location using the default MapKit style.

### Annotations in SwiftUI

struct MapMarker

A balloon-shaped annotation used to indicate the location on a map.

Deprecated

struct MapPin

A pin-shaped annotation used to indicate a location on a map.

Deprecated

struct MapAnnotation

A customizable annotation that marks a map location.

Deprecated

protocol MapAnnotationProtocol

A protocol that represents the possible return types of annotations.

### Shared behavior

class MKPlacemark

A user-friendly description of a location on the map.

protocol MKAnnotation

An interface for associating your content with a specific map location.

class MKAnnotationView

The visual representation of one of your annotation objects.

## See Also

### Annotations and overlays

MapKit overlays

Create overlays to highlight geographic regions or paths.

