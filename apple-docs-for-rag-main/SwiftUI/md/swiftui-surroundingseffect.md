

- SwiftUI
-  SurroundingsEffect 

Structure

# SurroundingsEffect

Effects that the system can apply to passthrough video.

visionOS 1.0+

``` source
struct SurroundingsEffect
```

## Overview

Use one of these values with the preferredSurroundingsEffect(_:) view modifier to indicate what effect to apply to passthrough video when the modified view is displayed.

## Topics

### Getting the effect

static var systemDark: SurroundingsEffect

An effect that dims passthrough video.

Deprecated

### Type Properties

static var dark: SurroundingsEffect

An effect that dims passthrough video.

static var semiDark: SurroundingsEffect

An effect that dims passthrough video less than dark.

static var ultraDark: SurroundingsEffect

An effect that dims passthrough video more than dark

### Type Methods

static func colorMultiply(Color) -> SurroundingsEffect

An effect that applies a custom tint to the passthrough video by multiplying the passthrough with a Color.

static func dim(intensity: Double) -> SurroundingsEffect

An effect that dims the passthrough video a custom amount.

## Relationships

### Conforms To

- Equatable

## See Also

### Configuring passthrough

func preferredSurroundingsEffect(SurroundingsEffect?) -> some View

Applies an effect to passthrough video.

