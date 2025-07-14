

- MapKit
-  MKOverlay 

Protocol

# MKOverlay

An interface for associating content with a specific map region.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
protocol MKOverlay : MKAnnotation
```

## Overview

*Overlay objects* are data objects that define the geographic data to cover. MapKit defines several concrete classes that adopt this protocol and define standard shapes like rectangles, circles, and polygons. You might use overlays to define the geographic boundaries of a national park or trace a bus route along city streets. You add an overlay to your map view by calling its addOverlay(_:) method or any other map view method for adding overlays to the map. When the overlay’s region intersects the visible portion of the map, the map view calls the mapView(_:rendererFor:) method of its delegate to obtain the renderer object responsible for drawing the overlay.

If you add an overlay to a map view as an annotation, instead of adding it as an overlay, the map view treats your overlay as an annotation. Specifically, it displays your overlay only when its coordinate is in the visible map region, rather than displaying the overlay when any portion of its covered area is visible.

## Topics

### Describing the overlay geometry

var coordinate: CLLocationCoordinate2D

The approximate center point of the overlay area.

**Required**

var boundingMapRect: MKMapRect

The projected rectangle that encompasses the overlay.

**Required**

### Determining map intersections

func intersects(MKMapRect) -> Bool

Returns a Boolean value that indicates whether the specified rectangle intersects the overlay’s shape.

### Optimizing map rendering

func canReplaceMapContent() -> Bool

Returns a Boolean value that indicates whether the overlay content replaces the underlying map content.

## Relationships

### Inherits From

- MKAnnotation
- NSObjectProtocol

### Conforming Types

- MKCircle
- MKGeodesicPolyline
- MKMultiPolygon
- MKMultiPolyline
- MKPolygon
- MKPolyline
- MKTileOverlay

## See Also

### Shared behavior

class MKOverlayRenderer

The shared infrastructure for drawing overlays on the map surface.

class MKShape

An abstract class that defines the basic properties for all shape-based overlay objects.

class MKMultiPoint

An abstract class that defines the common behavior that open and closed polygon overlays share.

class MKPlacemark

A user-friendly description of a location on the map.

