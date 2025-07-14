

- MapKit
-  MKGradientPolylineRenderer 

Class

# MKGradientPolylineRenderer

A visual representation of any polyline overlay object with a gradient.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MKGradientPolylineRenderer
```

## Overview

This renderer only applies a stroke to the line; it doesn’t fill it. Set the gradients with setColors:atLocations: and pair colors to locations that MapKit represents as unit distance values along the distance of the polyline. Don’t subclass `MKGradientPolylineRenderer`. Use the class as-is.

The gradient displays itself along the direction of the line.

## Topics

### Accessing the gradient colors

func setColors([UIColor], locations: [CGFloat])

Sets the iOS colors and corresponding unit distance values to create gradients.

func setColors([NSColor], locations: [CGFloat])

Sets the macOS colors and corresponding unit distance values to create gradients.

var colors: [UIColor]

An array that represents the gradient’s color transition points.

var locations: [CGFloat]

An array of location indexes that correspond to their respective colors.

## Relationships

### Inherits From

- MKPolylineRenderer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

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

