

- Foundation
-  NSEdgeInsets 

Structure

# NSEdgeInsets

A description of the distance between the edges of two rectangles.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct NSEdgeInsets
```

## Overview

Edge insets describe the distance between the edges of one rectangle to a related rectangle that can be described by measuring a constant but edge-specific distance from each edge.

A common use for this structure is to describe the relationship between a view’s frame and its alignment rectangle.

## Topics

### Creating an edge insets structure

init(top: Double, left: Double, bottom: Double, right: Double)

Creates an edge insets structure with the specified inset values.

func NSEdgeInsetsMake(Double, Double, Double, Double) -> NSEdgeInsets

Creates an edge insets structure with the specified inset values.

init()

Creates an edge insets structure.

### Specifying the edge insets

var bottom: Double

The distance from the bottom of the source rectangle to the bottom of the result rectangle.

var left: Double

The distance from the left side of the source rectangle to the left side of the result rectangle.

var right: Double

The distance from the right side of the source rectangle to the right side of the result rectangle.

var top: Double

The distance from the top of the source rectangle to the top of the result rectangle.

### Comparing edge insets

func NSEdgeInsetsEqual(NSEdgeInsets, NSEdgeInsets) -> Bool

Returns a Boolean value that indicates whether two edge insets structures are equal.

### Getting the zero constant

let NSEdgeInsetsZero: NSEdgeInsets

An edge insets structure with a zero inset on each edge.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Geometry

@frozen struct CGFloat

The basic type for floating-point scalar values in Core Graphics and related frameworks.

typealias NSPoint

A point in a Cartesian coordinate system.

typealias NSSize

A two-dimensional size.

typealias NSRect

A rectangle.

struct AffineTransform

A graphics coordinate transformation.

