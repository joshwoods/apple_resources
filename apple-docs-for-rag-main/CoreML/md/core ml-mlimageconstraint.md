

- Core ML
-  MLImageConstraint 

Class

# MLImageConstraint

The width, height, and pixel format constraints of an image feature.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class MLImageConstraint
```

## Overview

In CoreML, an *image* is a collection of pixels represented by CVPixelBuffer (Swift) or CVPixelBuffer (Objective-C). An *image feature* is a model input or output that accepts or produces, respectively, an image bundled in an MLFeatureValue. `MLImageConstraint` defines the image feature’s limitations for the images within an `MLFeatureValue`.

If a model has an image feature for an input or output, the model author uses an *image feature description* by creating an MLFeatureDescription. The feature description for an image input or output has:

- Its type property set to MLFeatureType.image

- Its imageConstraint property set to an MLImageConstraint instance configured to the image feature’s size and format

Image features that support additional image sizes provide a range of sizes, or a list of discrete sizes, in their image constraint’s sizeConstraint property.

## Topics

### Accessing the Constraints

var pixelsWide: Int

The model’s default width for an image feature.

var pixelsHigh: Int

The model’s default height for an image feature.

var pixelFormatType: OSType

The model’s pixel format for an image feature.

### Inspecting Acceptable Sizes

var sizeConstraint: MLImageSizeConstraint

Additional sizes this image feature supports.

class MLImageSizeConstraint

A list or range of sizes that augment an image constraint’s default size.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Creating Image Feature Values

convenience init(pixelBuffer: CVPixelBuffer)

Creates a feature value that contains an image from a pixel buffer.

convenience init(CGImage: CGImage, pixelsWide: Int, pixelsHigh: Int, pixelFormatType: OSType, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by a core graphics image and its size and pixel format.

convenience init(CGImage: CGImage, orientation: CGImagePropertyOrientation, pixelsWide: Int, pixelsHigh: Int, pixelFormatType: OSType, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by a core graphics image and its orientation, size, and pixel format.

convenience init(CGImage: CGImage, constraint: MLImageConstraint, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by a core graphics image and a constraint.

convenience init(CGImage: CGImage, orientation: CGImagePropertyOrientation, constraint: MLImageConstraint, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by a core graphics image, an orientation, and a constraint.

convenience init(imageAtURL: URL, pixelsWide: Int, pixelsHigh: Int, pixelFormatType: OSType, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by an image URL and the image’s size and pixel format.

convenience init(imageAtURL: URL, orientation: CGImagePropertyOrientation, pixelsWide: Int, pixelsHigh: Int, pixelFormatType: OSType, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by an image URL and the image’s orientation, size, and pixel format.

convenience init(imageAtURL: URL, constraint: MLImageConstraint, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by an image URL and a constraint.

convenience init(imageAtURL: URL, orientation: CGImagePropertyOrientation, constraint: MLImageConstraint, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by an image URL, an orientation, and a constraint.

struct ImageOption

The initializer options you use to crop and scale an image when creating an image feature value.

