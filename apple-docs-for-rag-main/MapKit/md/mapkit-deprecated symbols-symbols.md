

- MapKit
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

MapKit classes, protocols, and entitlements that are no longer supported.

## Topics

### Classes

class MKCircleView

Provides the visual representation for an MKCircle annotation object.

Deprecated

class MKOverlayView

Defines the basic behavior associated with all overlay views.

Deprecated

class MKOverlayPathView

Represents a generic overlay that draws its contents using a Core Graphics path data type.

Deprecated

class MKPolygonView

Provides the visual representation for an MKPolygon annotation object.

Deprecated

class MKPolylineView

Provides the visual representation for an MKPolyline annotation object.

Deprecated

class MKPinAnnotationView

An annotation view that displays a pin image on the map.

Deprecated

### Properties

var filterType: MKLocalSearchCompleter.FilterType

The filter options for the search results.

Deprecated

var pinColor: MKPinAnnotationColor

The color of the pin head.

Deprecated

var showsPointsOfInterest: Bool

A Boolean value that indicates whether the map displays point-of-interest information.

Deprecated

var showsPointsOfInterest: Bool

A Boolean value that indicates whether the map displays point-of-interest information.

Deprecated

var mapType: MKMapType

The map’s visual style.

Deprecated

### Methods

func view(for: any MKOverlay) -> MKOverlayView

Returns the view associated with the overlay object, if any.

Deprecated

func mapView(MKMapView, didAddOverlayViews: [Any])

Tells the delegate when the map adds one or more overlay views to the map.

Deprecated

func mapView(MKMapView, viewFor: any MKOverlay) -> MKOverlayView

Asks the delegate for the overlay view to use when displaying the specified overlay object.

Deprecated

### Protocols

struct MapPin

A pin-shaped annotation used to indicate a location on a map.

Deprecated

### Enumerations

enum FilterType

Constants indicating the types of search completions to return.

Deprecated

enum MKMapType

The type of map to display.

Deprecated

enum MKPinAnnotationColor

The supported colors for pin annotations.

Deprecated

### Entitlements

Maps Entitlement

A Boolean value that indicates whether the app may provide directions beyond what Maps supports, such as subway routes, hiking trails, and bike paths.

Deprecated

