

- MapKit
-  MKDistanceFormatter 

Class

# MKDistanceFormatter

A utility object that converts between a geographic distance and a string-based expression of that distance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
class MKDistanceFormatter
```

## Overview

Use a distance formatter to display distances to the user or to parse user-specified text to obtain a numerical value for a distance. When formatting strings containing distances, a distance formatter object takes into account the user’s locale and language settings. You can also specify a custom locale or custom units for any distances that you format.

## Topics

### Converting distances

func string(fromDistance: CLLocationDistance) -> String

Creates a string representation of the specified distance.

func distance(from: String) -> CLLocationDistance

Returns the distance value parsed from the specified string.

### Specifying the format

var locale: Locale!

The locale to use when formatting strings.

var units: MKDistanceFormatter.Units

The measuring system — imperial or metric — to use for units.

enum Units

Constants that reflect the type of units to use in the string.

var unitStyle: MKDistanceFormatter.DistanceUnitStyle

The preferred style for units.

enum DistanceUnitStyle

Constants that indicate the format style to use for strings.

## Relationships

### Inherits From

- Formatter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Map coordinates

struct MKCoordinateRegion

A rectangular geographic region that centers around a specific latitude and longitude.

struct MKCoordinateSpan

The width and height of a map region.

struct MKMapRect

A rectangular area on a two-dimensional map projection.

struct MKMapPoint

A point on a two-dimensional map projection.

struct MKMapSize

Width and height information on a two-dimensional map projection.

