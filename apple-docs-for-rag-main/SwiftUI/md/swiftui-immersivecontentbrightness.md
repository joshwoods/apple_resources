

- SwiftUI
-  ImmersiveContentBrightness 

Structure

# ImmersiveContentBrightness

The content brightness of an immersive space.

visionOS 1.0+

``` source
struct ImmersiveContentBrightness
```

## Overview

Use a value of this type as an input to the immersiveContentBrightness(_:) scene modifier to indicate the ambient content brightness of an ImmersiveSpace.

When you do this to create an environment that’s suitable for video playback, use one of the standard brightness values like bright, dim, or dark to provide good results for most use cases. To optimize further, you can create a custom brightness using a normalized value that expresses the linear brightness ratio between a standard dynamic range white video frame and the background that surrounds the player window.

## Topics

### Type Properties

static let automatic: ImmersiveContentBrightness

The default content brightness.

static let bright: ImmersiveContentBrightness

A bright content brightness.

static let dark: ImmersiveContentBrightness

A dark content brightness.

static let dim: ImmersiveContentBrightness

A dimmed content brightness.

### Type Methods

static func custom(Double) -> ImmersiveContentBrightness

Creates a content brightness with a custom value.

## Relationships

### Conforms To

- Equatable

## See Also

### Adjusting content brightness

func immersiveContentBrightness(ImmersiveContentBrightness) -> some Scene

Sets the content brightness of an immersive space.

