

- Create ML Components
-  RandomImageNoiseGenerator 

Structure

# RandomImageNoiseGenerator

A transformer that adds random noise to an image.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct RandomImageNoiseGenerator
```

## Topics

### Creating a noise generator

init(intensity: Double)

Creates transformer that generates random noise to apply to an image.

### Getting the intensity

var intensity: Double

The intensity of the random noise to add to the image.

### Performing the transformation

func applied(to: CIImage, eventHandler: EventHandler?) -> CIImage

Adds random noise to the input image.

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

struct ImageRotator

An image rotating transformer.

struct MLModelImageFeatureExtractor

An image feature extractor provided by an MLModel.

