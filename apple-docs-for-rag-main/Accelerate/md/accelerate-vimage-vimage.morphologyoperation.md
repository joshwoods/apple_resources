

- Accelerate
- vImage
-  vImage.MorphologyOperation 

Enumeration

# vImage.MorphologyOperation

Describes which morphology operation to perform.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
enum MorphologyOperation
```

## Topics

### Enumeration Cases

case dilate(structuringElement: vImage.ConvolutionKernel2D&lt;ComponentType>)

Applies dilation using a structuring element.

case erode(structuringElement: vImage.ConvolutionKernel2D&lt;ComponentType>)

Applies erosion using a structuring element.

case maximize(kernelSize: vImage.Size)

Maximizes using an implicit kernel of a specified size.

case minimize(kernelSize: vImage.Size)

Minimizes using an implicit kernel of a specified size.

### Instance Properties

var structuringElement: vImage.ConvolutionKernel2D&lt;ComponentType>?

The dilation or erosion structuring element.

var height: vImagePixelCount

The height of the morphology kernel.

var width: vImagePixelCount

The width of the morphology kernel.

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

enum Gamma

Describes either a used-defined or constant gamma.

enum ReflectionAxis

The axis to reflect an image.

enum Rotation

The angle to rotate an image.

enum ShearDirection

The shear direction.

