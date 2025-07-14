

- MapKit
-  MKMapRect 

Structure

# MKMapRect

A rectangular area on a two-dimensional map projection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MKMapRect
```

## Overview

If you project the curved surface of the globe onto a flat surface, what you get is a two-dimensional version of a map where longitude lines appear to be parallel. Such maps are often used to show the entire surface of the globe all at once. An `MKMapRect` data structure represents a rectangular area as seen on this two-dimensional map.

## Topics

### Creating a map rectangle

init()

Creates the rectangle with an empty region.

init(origin: MKMapPoint, size: MKMapSize)

Creates the map rectangle with the specified point and size.

init(x: Double, y: Double, width: Double, height: Double)

Creates a new map rectangle structure from the specified values.

init(MKMapRect)

Returns the region that corresponds to the specified map rectangle.

### Getting standard map rectangles

static let null: MKMapRect

The null map rectangle.

static let world: MKMapRect

The map rectangle that represents the world in the two-dimensional map projection.

### Getting the rectangle coordinates

var origin: MKMapPoint

The origin point of the rectangle.

var size: MKMapSize

The width and height of the rectangle, starting from the origin point.

### Getting the boundaries

var minX: Double

Returns the minimum x-axis value of the specified rectangle.

var minY: Double

Returns the minimum y-axis value of the specified rectangle.

var midX: Double

Returns the mid-point along the x-axis of the specified rectangle.

var midY: Double

Returns the mid-point along the y-axis of the specified rectangle.

var maxX: Double

Returns the maximum x-axis value of the specified rectangle.

var maxY: Double

Returns the maximum y-axis value of the specified rectangle.

var width: Double

Returns the width of the map rectangle.

var height: Double

Returns the height of the map rectangle.

### Comparing rectangles

var isNull: Bool

A Boolean value that indicates whether the specified rectangle is null.

func MKMapRectEqualToRect(MKMapRect, MKMapRect) -> Bool

Returns a Boolean value that indicates whether two map rectangles are equal.

var isEmpty: Bool

A Boolean value that indicates whether the specified rectangle has no area.

var spans180thMeridian: Bool

A Boolean value that indicates whether the specified map rectangle crosses the 180th meridian.

var remainder: MKMapRect

A rectangle that represents the normalized portion of the specified rectangle that lies outside the world map boundaries.

### Intersecting the rectangle

func contains(MKMapPoint) -> Bool

Returns a Boolean value that indicates whether the specified map point lies within the rectangle.

func contains(MKMapRect) -> Bool

Returns a Boolean value that indicates whether one rectangle contains another.

func intersects(MKMapRect) -> Bool

Returns a Boolean value that indicates whether two rectangles intersect each other.

### Modifying the rectangle

func union(MKMapRect) -> MKMapRect

Returns a rectangle that represents the union of two rectangles.

func intersection(MKMapRect) -> MKMapRect

Returns the rectangle that represents the intersection of two rectangles.

func insetBy(dx: Double, dy: Double) -> MKMapRect

Returns the specified rectangle with an inset by the specified amounts.

func offsetBy(dx: Double, dy: Double) -> MKMapRect

Returns a rectangle with an origin point that shifts by the specified amount.

func MKMapRectDivide(MKMapRect, UnsafeMutablePointer&lt;MKMapRect>, UnsafeMutablePointer&lt;MKMapRect>, Double, CGRectEdge)

Divides the specified rectangle into two smaller rectangles.

### Getting a description of the rectangle

func MKStringFromMapRect(MKMapRect) -> String

Returns a formatted string for the specified map rectangle.

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

struct MKMapPoint

A point on a two-dimensional map projection.

struct MKMapSize

Width and height information on a two-dimensional map projection.

class MKDistanceFormatter

A utility object that converts between a geographic distance and a string-based expression of that distance.

