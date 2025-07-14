

- SwiftUI
-  Capsule 

Structure

# Capsule

A capsule shape aligned inside the frame of the view containing it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Capsule
```

## Overview

A capsule shape is equivalent to a rounded rectangle where the corner radius is chosen as half the length of the rectangle’s smallest edge.

## Topics

### Creating a capsule

init(style: RoundedCornerStyle)

Creates a new capsule shape.

### Getting the shape’s characteristics

var style: RoundedCornerStyle

## Relationships

### Conforms To

- Animatable
- Copyable
- InsettableShape
- Sendable
- Shape
- View

## See Also

### Creating circular shapes

struct Circle

A circle centered on the frame of the view containing it.

struct Ellipse

An ellipse aligned inside the frame of the view containing it.

