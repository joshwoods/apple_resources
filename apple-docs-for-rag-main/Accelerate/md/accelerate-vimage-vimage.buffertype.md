

- Accelerate
- vImage
-  vImage.BufferType 

Enumeration

# vImage.BufferType

Codes that represent vImage buffer types.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum BufferType
```

## Topics

### Initializers

init?(bufferTypeCode: Int, model: CGColorSpaceModel?)

Creates a buffer type enumeration from the specified code and color space model.

### Enumeration Cases

case Cb

The buffer contains the blue chrominance channel.

case Cr

The buffer contains the red chrominance channel.

case YCbCr

The buffer contains interleaved luminance and both chroma channels.

case alpha

The buffer contains the alpha channel or coverage component.

case chroma

The buffer contains the interleaved chrominance channels.

case chunky

The buffer contains chunky data.

case cmykBlack

The buffer contains the black channel.

case cmykCyan

The buffer contains the cyan channel.

case cmykMagenta

The buffer contains the magenta channel.

case cmykYellow

The buffer contains the yellow channel.

case coreGraphics

The buffer contains a Core Graphics image.

case indexed

The buffer contains data in an indexed colorspace.

case labA

The buffer contains the `a*` channel.

case labB

The buffer contains the `b*` channel.

case labL

The buffer contains the `L*` channel.

case luminance

The buffer contains only luminance data.

case monochrome

The buffer contains monochrome data.

case rgbBlue

The buffer contains the blue channel.

case rgbGreen

The buffer contains the green channel.

case rgbRed

The buffer contains the red channel.

case xyzX

The buffer contains the `X` channel.

case xyzY

The buffer contains the `Y` channel.

case xyzZ

The buffer contains the `Z` channel.

### Buffer Type Properties

var bufferTypeCode: vImageBufferTypeCode

The type code of the buffer type.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Enumerations

enum BlendMode

Constants that specify an alpha blending mode.

enum ChannelOrdering

Constants that specify the channel ordering of a pixel buffer.

enum CompositeMode

Constants that specify whether the format of layers is premultiplied or nonpremultiplied.

enum EdgeMode

Constants that specify edge modes for convolution operations.

enum Error

An error that occurs during a vImage operation.

enum FloodFillConnectivity

enum Gamma

Describes either a used-defined or constant gamma.

enum MorphologyOperation

Describes which morphology operation to perform.

enum ReflectionAxis

The axis to reflect an image.

enum Rotation

The angle to rotate an image.

enum ShearDirection

The shear direction.

