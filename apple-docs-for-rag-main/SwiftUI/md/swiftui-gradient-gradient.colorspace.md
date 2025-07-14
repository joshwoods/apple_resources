

- SwiftUI
- Gradient
-  Gradient.ColorSpace 

Structure

# Gradient.ColorSpace

A method of interpolating between the colors in a gradient.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ColorSpace
```

## Topics

### Getting an interpolation method

static let device: Gradient.ColorSpace

Interpolates gradient colors in the output color space.

static let perceptual: Gradient.ColorSpace

Interpolates gradient colors in a perceptual color space.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Working with color spaces

func colorSpace(Gradient.ColorSpace) -> AnyGradient

Returns a version of the gradient that will use a specified color space for interpolating between its colors.

