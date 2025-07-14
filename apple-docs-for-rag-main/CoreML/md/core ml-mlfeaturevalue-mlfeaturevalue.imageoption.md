

- Core ML
- MLFeatureValue
-  MLFeatureValue.ImageOption 

Structure

# MLFeatureValue.ImageOption

The initializer options you use to crop and scale an image when creating an image feature value.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
struct ImageOption
```

## Topics

### Image Options Keys

static let cropRect: MLFeatureValue.ImageOption

The option you use to crop an image when creating an image feature value.

static let cropAndScale: MLFeatureValue.ImageOption

The option you use to crop and scale an image when creating an image feature value.

### Image Option Key Initializers

init(String)

Creates an image feature option key from a string.

init(rawValue: String)

Creates an image feature option key from a raw value string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

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

class MLImageConstraint

The width, height, and pixel format constraints of an image feature.

