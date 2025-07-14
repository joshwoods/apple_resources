

- SpriteKit
-  SKRange 

Class

# SKRange

A definition of a range of floating-point values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class SKRange
```

## Overview

You typically use a SKRange to clamp a value so that it is within the specified range.

## Topics

### Creating a Range Object

convenience init(value: CGFloat, variance: CGFloat)

Creates and initializes a new range object using a value and a maximum distance from that value.

class func withNoLimits() -> Self

Creates and initializes a new range object that encompasses all possible values.

convenience init(lowerLimit: CGFloat)

Creates and initializes a new range object that specifies only a minimum value.

convenience init(upperLimit: CGFloat)

Creates and initializes a new range object that specifies only a maximum value.

convenience init(constantValue: CGFloat)

Creates and initializes a new range object that specifies a constant value.

init(lowerLimit: CGFloat, upperLimit: CGFloat)

Initializes a new range object.

### Inspecting a Range Object’s Limits

var lowerLimit: CGFloat

The minimum possible value.

var upperLimit: CGFloat

The maximum possible value.

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

class SKRegion

The definition of an arbitrary area.

