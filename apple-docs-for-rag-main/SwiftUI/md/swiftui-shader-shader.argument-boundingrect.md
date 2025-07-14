

- SwiftUI
- Shader
- Shader.Argument
-  boundingRect 

Type Property

# boundingRect

Returns an argument value representing the bounding rect of the shape or view that the shader is attached to, as `float4(x, y, width, height)`. This value is undefined for shaders that do not have a natural bounding rect (e.g. filter effects drawn into `GraphicsContext`).

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
static var boundingRect: Shader.Argument { get }
```

## See Also

### Creating argument values

static func color(Color) -> Shader.Argument

Returns an argument value representing `color`. When passed to a MSL function it will convert to a `half4` value, as a premultiplied color in the target color space.

static func colorArray([Color]) -> Shader.Argument

Returns an argument value defined by the provided array of color values. When passed to an MSL function it will convert to a `device const half4 *ptr, int count` pair of parameters.

static func data(Data) -> Shader.Argument

Returns an argument value defined by the provided data value. When passed to an MSL function it will convert to a `device const void *ptr, int size_in_bytes` pair of parameters.

static func float&lt;T>(T) -> Shader.Argument

Returns an argument value representing the MSL value `float(x)`.

static float2(_:)

Returns an argument value representing the MSL value `float2(point.x, point.y)`.

static func float2&lt;T>(T, T) -> Shader.Argument

Returns an argument value representing the MSL value `float2(x, y)`.

static func float3&lt;T>(T, T, T) -> Shader.Argument

Returns an argument value representing the MSL value `float3(x, y, z)`.

static func float4&lt;T>(T, T, T, T) -> Shader.Argument

Returns an argument value representing the MSL value `float4(x, y, z, w)`.

static func floatArray([Float]) -> Shader.Argument

Returns an argument value defined by the provided array of floating point numbers. When passed to an MSL function it will convert to a `device const float *ptr, int count` pair of parameters.

static func image(Image) -> Shader.Argument

Returns an argument value defined by the provided image. When passed to an MSL function it will convert to a `texture2d` value. Currently only one image parameter is supported per `Shader` instance.

