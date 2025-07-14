

- SwiftUI
-  GlassBackgroundDisplayMode 

Enumeration

# GlassBackgroundDisplayMode

The display mode of a glass background.

visionOS 1.0+

``` source
enum GlassBackgroundDisplayMode
```

## Overview

Use a value of this type to indicate when to display a glass background that you add to a view using a view modifier like glassBackgroundEffect(displayMode:).

## Topics

### Getting the mode

case always

Always display the glass material.

case implicit

Display the glass material only when the view isn’t already contained in glass.

case never

Never display the glass material.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Adding a glass background

func glassBackgroundEffect(displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with an automatic glass background effect and container-relative rounded rectangle shape.

func glassBackgroundEffect&lt;S>(in: S, displayMode: GlassBackgroundDisplayMode) -> some View

Fills the view’s background with an automatic glass background effect and a shape that you specify.

