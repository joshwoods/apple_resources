

- MapKit
-  MKCircle 

Class

# MKCircle

A circular overlay with a configurable radius that you center on a geographic coordinate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKCircle
```

## Overview

This class defines the portion of the map that the overlay covers. To draw the region, return an MKCircleRenderer object from the mapView(_:rendererFor:) method of your map view delegate.

## Topics

### Creating a circle overlay

convenience init(center: CLLocationCoordinate2D, radius: CLLocationDistance)

Creates and returns a circle object using the specified coordinate and radius.

convenience init(mapRect: MKMapRect)

Creates and returns a circle object that derives the circular area from the specified rectangle.

### Accessing the overlay’s attributes

var coordinate: CLLocationCoordinate2D

The center point of the circular area, specified as a latitude and longitude.

var radius: CLLocationDistance

The radius of the circular area, in meters.

var boundingMapRect: MKMapRect

The bounding rectangle of the circular area.

## Relationships

### Inherits From

- MKShape

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- MKOverlay
- NSObjectProtocol

## See Also

### Circular overlays

class MKCircleRenderer

The visual representation of a circular overlay.

