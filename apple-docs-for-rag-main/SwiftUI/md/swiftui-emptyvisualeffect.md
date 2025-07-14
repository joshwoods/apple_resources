

- SwiftUI
-  EmptyVisualEffect 

Structure

# EmptyVisualEffect

The base visual effect that you apply additional effect to.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct EmptyVisualEffect
```

## Overview

`EmptyVisualEffect` does not change the appearance of the view that it is applied to.

## Topics

### Creating an empty visual effect

init()

Creates a new empty visual effect.

## Relationships

### Conforms To

- Animatable
- Sendable
- VisualEffect

## See Also

### Applying effects based on geometry

func visualEffect((EmptyVisualEffect, GeometryProxy) -> some VisualEffect) -> some View

Applies effects to this view, while providing access to layout information through a geometry proxy.

func visualEffect3D((EmptyVisualEffect, GeometryProxy3D) -> some VisualEffect) -> some View

Applies effects to this view, while providing access to layout information through a 3D geometry proxy.

protocol VisualEffect

Visual Effects change the visual appearance of a view without changing its ancestors or descendents.

