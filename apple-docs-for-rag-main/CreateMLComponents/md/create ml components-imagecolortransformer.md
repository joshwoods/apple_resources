

- Create ML Components
-  ImageColorTransformer 

Structure

# ImageColorTransformer

An image color transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct ImageColorTransformer
```

## Topics

### Creating a color transformer

init(brightness: Float?, contrast: Float?, hue: Float?, saturation: Float?)

Creates an image color transformer.

### Getting the properties

var brightness: Float?

The brightness adjustment, between 0.0 and 1.0.

var contrast: Float?

The contrast adjustment, between 0.0 and 1.0.

var hue: Float?

The hue adjustment, between 0.0 and 1.0.

var saturation: Float?

The saturation adjustment, between 0.0 and 1.0.

### Applying the transformation

func applied(to: CIImage, eventHandler: EventHandler?) -> CIImage

Performs the image color transformation operation on the input image.

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

