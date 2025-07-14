

- MapKit
-  MKCircleRenderer 

Class

# MKCircleRenderer

The visual representation of a circular overlay.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKCircleRenderer
```

## Overview

This renderer fills and strokes the circular region that the overlay object represents. You can change the color and other drawing attributes of the circle by modifying the properties it inherits from the main class. You typically use this class as-is and don’t subclass it.

You create an instance of this class in your map view delegate’s mapView(_:rendererFor:) method.

## Topics

### Creating a circle renderer

init(circle: MKCircle)

Creates a new overlay view using the specified circle overlay object.

### Accessing the overlay object

var circle: MKCircle

The circle overlay object that contains the information for drawing the overlay.

### Accessing the stroke

var strokeStart: CGFloat

The unit distance along the circle where the stroke starts.

var strokeEnd: CGFloat

The unit distance along the circle where the stroke ends.

## Relationships

### Inherits From

- MKOverlayPathRenderer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Circular overlays

class MKCircle

A circular overlay with a configurable radius that you center on a geographic coordinate.

