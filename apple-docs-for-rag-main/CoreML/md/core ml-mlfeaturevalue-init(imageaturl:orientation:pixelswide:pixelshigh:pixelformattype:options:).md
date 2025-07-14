

- Core ML
- MLFeatureValue
-  init(imageAtURL:orientation:pixelsWide:pixelsHigh:pixelFormatType:options:) 

Initializer

# init(imageAtURL:orientation:pixelsWide:pixelsHigh:pixelFormatType:options:)

Creates a feature value that contains an image defined by an image URL and the image’s orientation, size, and pixel format.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
convenience init(
    imageAtURL url: URL,
    orientation: CGImagePropertyOrientation,
    pixelsWide: Int,
    pixelsHigh: Int,
    pixelFormatType: OSType,
    options: [MLFeatureValue.ImageOption : Any]? = nil
) throws
```

``` source
convenience init(
    imageAt url: URL,
    orientation: CGImagePropertyOrientation,
    pixelsWide: Int,
    pixelsHigh: Int,
    pixelFormatType: OSType,
    options: [MLFeatureValue.ImageOption : Any]? = nil
) throws
```

## Parameters 

`url`  

A URL (Swift) or NSURL (Objective-C) to an image.

`orientation`  

A CGImagePropertyOrientation instance.

`pixelsWide`  

The image’s width in pixels.

`pixelsHigh`  

The image’s height in pixels.

`pixelFormatType`  

The image’s pixel format (see Pixel Format Identifiers).

`options`  

A dictionary of VNImageCropAndScaleOption values, each keyed by MLFeatureValue.ImageOption.

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

convenience init(imageAtURL: URL, constraint: MLImageConstraint, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by an image URL and a constraint.

convenience init(imageAtURL: URL, orientation: CGImagePropertyOrientation, constraint: MLImageConstraint, options: [MLFeatureValue.ImageOption : Any]?) throws

Creates a feature value that contains an image defined by an image URL, an orientation, and a constraint.

class MLImageConstraint

The width, height, and pixel format constraints of an image feature.

struct ImageOption

The initializer options you use to crop and scale an image when creating an image feature value.

