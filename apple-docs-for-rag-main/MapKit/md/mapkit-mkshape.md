

- MapKit
-  MKShape 

Class

# MKShape

An abstract class that defines the basic properties for all shape-based overlay objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKShape
```

## Overview

You can’t instantiate this class directly; use a subclass instead. Subclasses are responsible for defining the geometry of the shape and providing an appropriate value for the coordinate property they inherit from the MKAnnotation protocol.

## Topics

### Accessing the shape attributes

var title: String?

The title of the shape annotation.

var subtitle: String?

The subtitle of the shape annotation.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MKCircle
- MKMultiPoint
- MKMultiPolygon
- MKMultiPolyline
- MKPointAnnotation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- NSObjectProtocol

## See Also

### Shared behavior

protocol MKOverlay

An interface for associating content with a specific map region.

class MKOverlayRenderer

The shared infrastructure for drawing overlays on the map surface.

class MKMultiPoint

An abstract class that defines the common behavior that open and closed polygon overlays share.

class MKPlacemark

A user-friendly description of a location on the map.

