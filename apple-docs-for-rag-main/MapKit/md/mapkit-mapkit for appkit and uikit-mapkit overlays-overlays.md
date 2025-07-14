

- MapKit
- MapKit for AppKit and UIKit
-  MapKit overlays 

API Collection

# MapKit overlays

Create overlays to highlight geographic regions or paths.

## Topics

### Samples

Displaying overlays on a map

Add regions of layered content to a map view.

Displaying an updating path of a user’s location history

Continually update a MapKit overlay displaying the path a user travels.

### Circular overlays

class MKCircle

A circular overlay with a configurable radius that you center on a geographic coordinate.

class MKCircleRenderer

The visual representation of a circular overlay.

### Custom shape overlays

class MKPolygon

A closed polygon overlay.

class MKPolygonRenderer

The visual representation of a single polygon overlay.

class MKMultiPolygon

A collection of multiple closed polygon overlays.

class MKMultiPolygonRenderer

The visual representation of multiple polygon overlays.

class MKOverlayPathRenderer

The visual representation of a path-based overlay.

### Multiple segment lines

class MKPolyline

An open polygon overlay consisting of one or more connected line segments.

class MKGeodesicPolyline

An open polygon overlay consisting of line segments that follow the contours of the Earth to create the shortest path between the specified points.

class MKMultiPolyline

A collection of multipolyline shapes, each consisting of one or more connected line segments.

class MKPolylineRenderer

A visual representation of any polyline overlay object.

class MKMultiPolylineRenderer

A visual representation of multiple polyline overlay objects.

class MKGradientPolylineRenderer

A visual representation of any polyline overlay object with a gradient.

### Tiled image overlays

class MKTileOverlay

An overlay that covers an area of the map with tiles of bitmap images.

class MKTileOverlayRenderer

The renderer for a tile overlay that handles the drawing of bitmap images on the map surface.

### Shared behavior

protocol MKOverlay

An interface for associating content with a specific map region.

class MKOverlayRenderer

The shared infrastructure for drawing overlays on the map surface.

class MKShape

An abstract class that defines the basic properties for all shape-based overlay objects.

class MKMultiPoint

An abstract class that defines the common behavior that open and closed polygon overlays share.

class MKPlacemark

A user-friendly description of a location on the map.

## See Also

### Annotations and overlays

MapKit annotations

Create annotations to add indicators and additional details for specific locations on a map.

