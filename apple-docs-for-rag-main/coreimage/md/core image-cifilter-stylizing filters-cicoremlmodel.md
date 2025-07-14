

- Core Image
- CIFilter
- Stylizing Filters
-  CICoreMLModel 

Protocol

# CICoreMLModel

The properties you use to configure a Core ML model filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CICoreMLModel
```

## Topics

### Instance Properties

var headIndex: Float

A number that specifies which output of a multihead Core ML model applies the effect on the image.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var model: MLModel

The Core ML model used to apply the effect on the image.

**Required**

var softmaxNormalization: Bool

A Boolean value that specifies whether to apply Softmax normalization to the output of the model.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func coreMLModel() -> any CIFilter &amp; CICoreMLModel

Filters an image with a Core ML model.

