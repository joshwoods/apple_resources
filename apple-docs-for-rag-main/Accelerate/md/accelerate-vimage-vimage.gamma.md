

- Accelerate
- vImage
-  vImage.Gamma 

Enumeration

# vImage.Gamma

Describes either a used-defined or constant gamma.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
enum Gamma
```

## Topics

### User Defined Gamma

case fullPrecision(Float)

A user-defined gamma value with full-precision calculation.

case halfPrecision(Float)

A user-defined gamma value with half-precision calculation.

### Constant Gamma

case bt709ForwardHalfPrecision

ITU-R BT.709 standard.

case bt709ReverseHalfPrecision

ITU-R BT.709 standard reverse.

case elevenOverFiveHalfPrecision

Half-precision calculation using a gamma value of `11/5` or `2.2`.

case elevenOverNineHalfPrecision

Half-precision calculation using a gamma value of `11/9` or `(11/5)/(9/5)`.

case fiveOverElevenHalfPrecision

Half-precision calculation using a gamma value of `5/11` or `1/2.2`.

case fiveOverNineHalfPrecision

Half-precision calculation using a gamma value of `5/9` or `1/1.8`.

case nineOverElevenHalfPrecision

Half-precision calculation using a gamma value of `9/11` or `(9/5)/(11/5)`.

case nineOverFiveHalfPrecision

Half-precision calculation using a gamma value of `9/5` or `1.8`.

case sRGBForwardHalfPrecision

Half-precision calculation using the sRGB standard gamma value of `2.2`.

case sRGBReverseHalfPrecision

Half-precision calculation using the sRGB standard gamma value of `1/2.2`.

## See Also

### Enumerations

enum BlendMode

Constants that specify an alpha blending mode.

enum BufferType

Codes that represent vImage buffer types.

enum ChannelOrdering

Constants that specify the channel ordering of a pixel buffer.

enum CompositeMode

Constants that specify whether the format of layers is premultiplied or nonpremultiplied.

enum EdgeMode

Constants that specify edge modes for convolution operations.

enum Error

An error that occurs during a vImage operation.

enum FloodFillConnectivity

enum MorphologyOperation

Describes which morphology operation to perform.

enum ReflectionAxis

The axis to reflect an image.

enum Rotation

The angle to rotate an image.

enum ShearDirection

The shear direction.

