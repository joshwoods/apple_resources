

- Create ML Components
-  ImageScaler 

Structure

# ImageScaler

An image scaling transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct ImageScaler
```

## Topics

### Creating a transformer

init(targetSize: CGSize)

Creates an image scaler transformer. This transformer is used to scale an image to the `targetSize`.

init(targetHeight: Double)

Creates an image scaler transformer that preserves the aspect ratio.

init(targetWidth: Double)

Creates an image scaler transformer that preserves the aspect ratio.

### Getting the target image size

var targetSize: CGSize

The target image size.

### Performing the transformation

func applied(to: CIImage, eventHandler: EventHandler?) throws -> CIImage

Perform the image scaler operation on the input pixelBuffer.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
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

struct ImageRotator

An image rotating transformer.

struct RandomImageNoiseGenerator

A transformer that adds random noise to an image.

struct MLModelImageFeatureExtractor

An image feature extractor provided by an MLModel.

