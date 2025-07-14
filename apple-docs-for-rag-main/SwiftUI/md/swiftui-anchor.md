

- SwiftUI
-  Anchor 

Structure

# Anchor

An opaque value derived from an anchor source and a particular view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Anchor
```

## Overview

You can convert the anchor to a `Value` in the coordinate space of a target view by using a GeometryProxy to specify the target view.

## Topics

### Getting the anchor’s source

struct Source

A type-erased geometry value that produces an anchored value of a given type.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Accessing geometric constructs

enum Axis

The horizontal or vertical dimension in a 2D coordinate system.

struct Angle

A geometric angle whose value you access in either radians or degrees.

struct UnitPoint

A normalized 2D point in a view’s coordinate space.

struct UnitPoint3D

A normalized 3D point in a view’s coordinate space.

