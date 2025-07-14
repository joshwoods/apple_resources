

- SwiftUI
-  ShaderLibrary 

Structure

# ShaderLibrary

A Metal shader library.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@dynamicMemberLookup
struct ShaderLibrary
```

## Topics

### Getting the default shader library

static let `default`: ShaderLibrary

The default shader library of the main (i.e. app) bundle.

static func bundle(Bundle) -> ShaderLibrary

Returns the default shader library of the specified bundle.

### Creating a shader library

init(url: URL)

Creates a new Metal shader library from the contents of `url`, which must be the location of precompiled Metal library. Functions compiled from the returned library will only be cached as long as the returned library exists.

init(data: Data)

Creates a new Metal shader library from `data`, which must be the contents of precompiled Metal library. Functions compiled from the returned library will only be cached as long as the returned library exists.

### Access shader functions

static subscript(dynamicMember _: String) -> ShaderFunction

Returns a new shader function representing the stitchable MSL function called `name` in the default shader library.

### Subscripts

subscript(dynamicMember _: String) -> ShaderFunction

Returns a new shader function representing the stitchable MSL function in the library called `name`.

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

struct ShaderFunction

A reference to a function in a Metal shader library.

