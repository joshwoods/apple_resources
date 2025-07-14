

- Accelerate
- vImage
-  vImage.CompositeMode 

Enumeration

# vImage.CompositeMode

Constants that specify whether the format of layers is premultiplied or nonpremultiplied.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
enum CompositeMode
```

## Topics

### Enumeration Cases

case nonpremultiplied

Composite two non-premultiplied images, to produce a non-premultiplied result.

case nonpremultipliedToPremultiplied

Blends a nonpremultiplied top image into a premultiplied bottom image and returns a premultiplied result.

case premultiplied

Blends two premultiplied images to produce a premultiplied result.

case premultipliedWithConstantAlpha(ComponentType)

Performs premultiplied alpha compositing of two images, using a single alpha value for the entire image.

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Enumerations

enum BlendMode

Constants that specify an alpha blending mode.

enum BufferType

Codes that represent vImage buffer types.

enum ChannelOrdering

Constants that specify the channel ordering of a pixel buffer.

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

