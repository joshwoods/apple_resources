

- Core ML
- MLFeatureValue
-  init(pixelBuffer:) 

Initializer

# init(pixelBuffer:)

Creates a feature value that contains an image from a pixel buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
convenience init(pixelBuffer value: CVPixelBuffer)
```

## Parameters 

`value`  

A CVPixelBuffer (Swift) or CVPixelBuffer (Objective-C) instance.

## Discussion

Core ML supports different pixel format types depending on the model’s feature description. For information about `ImageFeatureType`, see Core ML Format Reference. When the image feature’s color space is `GRAYSCALE`, use kCVPixelFormatType_OneComponent8; and when it’s `GRAYSCALE_FLOAT16`, use kCVPixelFormatType_OneComponent16Half; otherwise, use kCVPixelFormatType_32BGRA when it’s set to `RGB` or `BGR`.

## See Also

### Creating Image Feature Values

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

class MLImageConstraint

The width, height, and pixel format constraints of an image feature.

struct ImageOption

The initializer options you use to crop and scale an image when creating an image feature value.

