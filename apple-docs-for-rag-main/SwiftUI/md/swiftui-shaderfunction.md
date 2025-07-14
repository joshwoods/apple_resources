

- SwiftUI
-  ShaderFunction 

Structure

# ShaderFunction

A reference to a function in a Metal shader library.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@dynamicCallable
struct ShaderFunction
```

## Topics

### Creating a shader function

init(library: ShaderLibrary, name: String)

Creates a new function reference from the provided shader library and function name string.

### Configuring a function

var library: ShaderLibrary

The shader library storing the function.

var name: String

The name of the shader function in the library.

func dynamicallyCall(withArguments: [Shader.Argument]) -> Shader

Returns a new shader by applying the provided argument values to the referenced function.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Accessing Metal shaders

func colorEffect(Shader, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a filter effect on the color of each pixel.

func distortionEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a geometric distortion effect on the location of each pixel.

func layerEffect(Shader, maxSampleOffset: CGSize, isEnabled: Bool) -> some View

Returns a new view that applies `shader` to `self` as a filter on the raster layer created from `self`.

struct Shader

A reference to a function in a Metal shader library, along with its bound uniform argument values.

struct ShaderLibrary

A Metal shader library.

