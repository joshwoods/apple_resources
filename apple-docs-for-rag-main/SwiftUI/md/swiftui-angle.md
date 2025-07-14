

- SwiftUI
-  Angle 

Structure

# Angle

A geometric angle whose value you access in either radians or degrees.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Angle
```

## Topics

### Getting constant angles

static var zero: Angle

static func degrees(Double) -> Angle

static func radians(Double) -> Angle

### Creating an angle

init()

init(degrees: Double)

init(radians: Double)

init(Angle2D)

### Getting the angle size

var degrees: Double

var radians: Double

## Relationships

### Conforms To

- Animatable
- BitwiseCopyable
- Comparable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Accessing geometric constructs

enum Axis

The horizontal or vertical dimension in a 2D coordinate system.

struct UnitPoint

A normalized 2D point in a view’s coordinate space.

struct UnitPoint3D

A normalized 3D point in a view’s coordinate space.

struct Anchor

An opaque value derived from an anchor source and a particular view.

