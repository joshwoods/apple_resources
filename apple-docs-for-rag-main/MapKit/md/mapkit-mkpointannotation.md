

- MapKit
-  MKPointAnnotation 

Class

# MKPointAnnotation

A string-based piece of location-specific data that you apply to a specific point on a map.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKPointAnnotation
```

## Overview

You use this class, rather than define a custom annotation object, in situations where all you want to do is display a title string at the specified point on the map.

## Topics

### Creating a Point Annotation

init()

Creates a map annotation that shows a title string at a point on a map.

### Accessing the Annotation’s Location

var coordinate: CLLocationCoordinate2D

The coordinate point of the annotation.

## Relationships

### Inherits From

- MKShape

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- MKGeoJSONObject
- NSObjectProtocol

## See Also

### Location annotations

Annotating a Map with Custom Data

Annotate a map with location-specific data using default and customized annotation views and callouts.

class MKMapItemAnnotation

An annotation that represents a map item

class MKMarkerAnnotationView

An annotation view that displays a balloon-shaped marker at the designated location.

class MKPinAnnotationView

An annotation view that displays a pin image on the map.

Deprecated

