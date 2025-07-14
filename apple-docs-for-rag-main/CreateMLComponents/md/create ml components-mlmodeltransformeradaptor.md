

- Create ML Components
-  MLModelTransformerAdaptor 

Structure

# MLModelTransformerAdaptor

A transformer that uses a Core ML model.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct MLModelTransformerAdaptor where Scalar : MLShapedArrayScalar, Scalar : BinaryFloatingPoint
```

## Topics

### Creating an adaptor

init(model: MLModel) throws

Creates a model adaptor from an MLModel.

init(contentsOf: URL, configuration: MLModelConfiguration) throws

Creates a model adaptor from a CoreML model URL.

### Getting the model

let model: MLModel

The CoreML model.

### Performing the transformation

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> MLShapedArray&lt;Scalar>

Performs a transformation on a single input.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

Transformer Implementations

## Relationships

### Conforms To

- Transformer

## See Also

### Core ML adaptors

struct MLModelClassifierAdaptor

A transformer that uses a Core ML model as a classifier.

struct MLModelRegressorAdaptor

A transformer that uses a Core ML model as a regressor.

struct ModelMetadata

User info keys that specify useful information about a model.

