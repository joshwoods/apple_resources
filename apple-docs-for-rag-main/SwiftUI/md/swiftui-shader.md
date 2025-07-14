

- SwiftUI
-  Shader 

Structure

# Shader

A reference to a function in a Metal shader library, along with its bound uniform argument values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct Shader
```

## Overview

Shader values can be used as filter effects on views, see the colorEffect(_:isEnabled:), distortionEffect(_:maxSampleOffset:isEnabled:), and layerEffect(_:maxSampleOffset:isEnabled:) functions.

Shaders also conform to the ShapeStyle protocol, letting their MSL shader function provide per-pixel color to fill any shape or text view. For a shader function to act as a fill pattern it must have a function signature matching:

```
[[ stitchable ]] half4 name(float2 position, args...)
```

where `position` is the user-space coordinates of the pixel applied to the shader, and `args...` should be compatible with the uniform arguments bound to `shader`. The function should return the premultiplied color value in the color space of the destination (typically extended sRGB).

## Topics

### Creating a shader

init(function: ShaderFunction, arguments: [Shader.Argument])

Creates a new shader from a function and the uniform argument values to bind to the function.

struct Argument

A single uniform argument value to a shader function.

### Getting the shader function

var function: ShaderFunction

The shader function called by the shader.

var arguments: [Shader.Argument]

The uniform argument values passed to the shader function.

### Configuring the shader

var dithersColor: Bool

For shader functions that return color values, whether the returned color has dither noise added to it, or is simply rounded to the output bit-depth. For shaders generating smooth gradients, dithering is usually necessary to prevent visible banding in the result.

### Structures

struct UsageType

The different ways in which a `Shader` may be used to render.

### Instance Methods

func compile(as: Shader.UsageType) async throws

Attempts to asynchronously compile a shader function, to minimize the chance of stalling when it is first used for rendering.

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable
- ShapeStyle

## See Also

### Accessing Metal shaders

func colorEffect(Shader, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a filter effect on the color of each pixel.

func distortionEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a geometric distortion effect on the location of each pixel.

func layerEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a filter on the raster layer created from `self`.

struct ShaderFunction

A reference to a function in a Metal shader library.

struct ShaderLibrary

A Metal shader library.

