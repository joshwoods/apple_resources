

- SwiftUI
-  MaterialActiveAppearance 

Structure

# MaterialActiveAppearance

The behavior for how materials appear active and inactive.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MaterialActiveAppearance
```

## Overview

On macOS, materials have active and inactive appearances that can reinforce the active appearance of the window they are in:

- Materials used as a `window` container background and `bar` materials will appear inactive when their containing window is inactive.

- All other materials will always appear active by default.

An explicit active appearance can be set to override a material’s default behavior. For example, materials used as the `window` container background can be made to always appear active by setting the active appearance behavior to be always active:

```
Text("Hello, World!")
    .containerBackground(
        Material.regular.materialActiveAppearance(.active),
        for: .window)
```

## Topics

### Type Properties

static let active: MaterialActiveAppearance

Materials will always appear active.

static let automatic: MaterialActiveAppearance

Materials will automatically appear active or inactive based on context and platform convention.

static let inactive: MaterialActiveAppearance

Materials will always appear inactive.

static let matchWindow: MaterialActiveAppearance

Materials will have an active or inactive appearance based on the active appearance of their window.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Transforming colors

func brightness(Double) -> some View

Brightens this view by the specified amount.

func contrast(Double) -> some View

Sets the contrast and separation between similar colors in this view.

func colorInvert() -> some View

Inverts the colors in this view.

func colorMultiply(Color) -> some View

Adds a color multiplication effect to this view.

func saturation(Double) -> some View

Adjusts the color saturation of this view.

func grayscale(Double) -> some View

Adds a grayscale effect to this view.

func hueRotation(Angle) -> some View

Applies a hue rotation effect to this view.

func luminanceToAlpha() -> some View

Adds a luminance to alpha effect to this view.

func materialActiveAppearance(MaterialActiveAppearance) -> some View

Sets an explicit active appearance for materials in this view.

var materialActiveAppearance: MaterialActiveAppearance

The behavior materials should use for their active state, defaulting to `automatic`.

