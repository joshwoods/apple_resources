

- MapKit
-  MKMapSize 

Structure

# MKMapSize

Width and height information on a two-dimensional map projection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MKMapSize
```

## Overview

If you project the curved surface of the globe onto a flat surface, what you get is a two-dimensional version of a map where longitude lines appear to be parallel. Such maps are often used to show the entire surface of the globe all at once. An `MKMapSize` data structure represents a horizontal and vertical distance as measured on this two-dimensional map.

## Topics

### Creating a map size

init()

Creates a map size that represents an empty area on a two-dimensional projection of a map.

init(width: Double, height: Double)

Creates a map size that represents an area on a two-dimensional projection of a map with the specified width and height.

### Getting standard map sizes

static let world: MKMapSize

The width and height, in map points, of the world in a two-dimensional map projection.

### Getting the width and height

var height: Double

The height of the specified area, measured in map points.

var width: Double

The width of the specified area, measured in map points.

### Comparing map sizes

func MKMapSizeEqualToSize(MKMapSize, MKMapSize) -> Bool

Returns a Boolean value that indicates whether two map sizes are equal.

### Getting a description of the size

func MKStringFromMapSize(MKMapSize) -> String

Returns a formatted string for the specified map size.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

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

class MKDistanceFormatter

A utility object that converts between a geographic distance and a string-based expression of that distance.

