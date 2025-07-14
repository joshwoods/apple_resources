

- SpriteKit
-  SKRegion 

Class

# SKRegion

The definition of an arbitrary area.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class SKRegion
```

## Overview

An SKRegion object defines a mathematical shape and is typically used to determine whether a particular point lies inside this area. For example, regions are used to define the area that a physics field can affect. Regions are defined using paths and mathematical shapes and can also be combined using constructive solid geometry.

## Topics

### Creating and Initializing Region Objects

class func infinite() -> Self

Returns a region that defines a region that includes all points.

init(size: CGSize)

Initializes a new region with a rectangular area.

init(radius: Float)

Initializes a new region with a circular area.

init(path: CGPath)

Initializes a new region using a Core Graphics path.

func inverse() -> Self

Returns a new region that is the mathematical inverse of an existing region.

func byDifference(from: SKRegion) -> Self

Returns a new region created by subtracting the contents of another region from this region.

func byIntersection(with: SKRegion) -> Self

Returns a new region created by intersecting the contents of this region with another region.

func byUnion(with: SKRegion) -> Self

Returns a new region created by combining the contents of this region with another region.

### Interacting with a Region

var path: CGPath?

Returns a Core Graphics path that defines the region.

func contains(CGPoint) -> Bool

Returns a Boolean value that indicates whether a particular point is contained in the region.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Mathematical Tools

class SKKeyframeSequence

An object that performs interpolation between values specified at different times (keyframes).

class SKRange

A definition of a range of floating-point values.

