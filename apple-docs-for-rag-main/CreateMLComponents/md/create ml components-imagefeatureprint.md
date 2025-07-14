

- Create ML Components
-  ImageFeaturePrint 

Structure

# ImageFeaturePrint

ImageFeaturePrint image feature extractor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct ImageFeaturePrint
```

## Topics

### Creating the extractor

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(cropAndScale: VNImageCropAndScaleOption, context: CIContext)

Creates a FeaturePrint feature extractor.

init(revision: Int, cropAndScale: VNImageCropAndScaleOption, context: CIContext)

Creates a FeaturePrint feature extractor.

### Getting the properties

let cropAndScale: VNImageCropAndScaleOption

The crop and scale options.

var revision: Int

The feature extractor revision number.

static let latestRevision: Int

The latest feature extractor revision.

### Performing the transformation

func applied(to: CIImage, eventHandler: EventHandler?) async throws -> MLShapedArray&lt;Float>

Extracts image features from an image.

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
- ImageFeatureExtractor
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

