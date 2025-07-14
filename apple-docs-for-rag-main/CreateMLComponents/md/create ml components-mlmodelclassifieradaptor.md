

- Create ML Components
-  MLModelClassifierAdaptor 

Structure

# MLModelClassifierAdaptor

A transformer that uses a Core ML model as a classifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct MLModelClassifierAdaptor where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint
```

## Topics

### Creating a transformer

init(model: MLModel) throws

Creates a MLModel classifier adaptor from a model.

init(contentsOf: URL, configuration: MLModelConfiguration) throws

Creates a model adaptor from a CoreML model URL.

### Getting the model

let model: MLModel

The CoreML model.

### Performing the transformation

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> ClassificationDistribution&lt;MLModelClassifierAdaptor&lt;Scalar>.Label>

Performs a prediction from a single input.

enum Label

The classifier label type.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

Transformer Implementations

## Relationships

### Conforms To

- Classifier
- Transformer

## See Also

### Core ML adaptors

struct MLModelTransformerAdaptor

A transformer that uses a Core ML model.

struct MLModelRegressorAdaptor

A transformer that uses a Core ML model as a regressor.

struct ModelMetadata

User info keys that specify useful information about a model.

