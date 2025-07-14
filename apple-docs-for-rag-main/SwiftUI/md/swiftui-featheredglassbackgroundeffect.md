

- SwiftUI
-  FeatheredGlassBackgroundEffect 

Structure

# FeatheredGlassBackgroundEffect

The feathered glass background effect.

visionOS 2.4+

``` source
struct FeatheredGlassBackgroundEffect
```

## Overview

You can also use feathered to construct this effect.

The layout size of a view with feathered glass background is based on the content size instead of the glass background size. When the glass background is clipped by an outer container, such as VStack or HStack, it can be resolved by incrasing content size, such as content padding, or reducing the feathered glass background size with its padding parameter.

## Topics

### Initializers

init()

Creates a feathered glassBackground effect.

init(padding: CGFloat, softEdgeRadius: CGFloat?)

Creates a feathered glassBackground effect.

## Relationships

### Conforms To

- GlassBackgroundEffect

