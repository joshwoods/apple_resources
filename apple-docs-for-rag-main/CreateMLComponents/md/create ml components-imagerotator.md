

- Create ML Components
-  ImageRotator 

Structure

# ImageRotator

An image rotating transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct ImageRotator
```

## Mentioned in 

Augmenting images to expand your training data

## Topics

### Creating the transformer

init(angle: Double)

Creates a transformer that rotates an image by a specified angle.

### Getting the angle

var angle: Double

The angle, in radians, by which to rotate the coordinate space of the specified context. Positive values rotate counterclockwise and negative values rotate clockwise.

### Performing the transformation

func applied(to: CIImage, eventHandler: EventHandler?) -> CIImage

Rotates the image and then scales and crops the rotated image to fit the extent of the input image.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

Transformer Implementations

## Relationships

### Conforms To

- Sendable
- Transformer

## See Also

### Image components

Augmenting images to expand your training data

Improve your model by using transformed versions of your training images.

Creating a multi-label image classifier

Train a machine learning model to assign multiple labels to an image.

struct ImageReader

An image file reader.

protocol ImageFeatureExtractor

A transformer that takes an image and outputs image features.

struct ImageCropper

An image crop transformer.

struct ImageScaler

An image scaling transformer.

struct ImageFeaturePrint

ImageFeaturePrint image feature extractor.

struct ImageBlur

An image blurring transformer.

struct ImageColorTransformer

An image color transformer.

struct ImageExposureAdjuster

An image exposure adjusting transformer.

struct ImageFlipper

An image flipper transformer.

struct RandomImageNoiseGenerator

A transformer that adds random noise to an image.

struct MLModelImageFeatureExtractor

An image feature extractor provided by an MLModel.

