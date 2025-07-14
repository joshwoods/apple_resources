

- Core ML
-  MLModelAsset 

Class

# MLModelAsset

An abstraction of a compiled Core ML model asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class MLModelAsset
```

## Overview

MLModelAsset provides a unified interface by abstracting the compiled model representations for `.mlmodelc` files and in-memory representations.

To use an in-memory model, create an MLModelAsset with an in-memory model specification, then call load(_:configuration:completionHandler:).

## Topics

### Creating a model asset

convenience init(specification: Data) throws

Creates a model asset from an in-memory model specification.

### Initializers

convenience init(specification: Data, blobMapping: [URL : Data]) throws

Construct a model asset from an ML Program specification by replacing blob file references with corresponding in-memory blobs.

convenience init(url: URL) throws

Constructs a ModelAsset from a compiled model URL.

### Instance Methods

func functionNames(completionHandler: ([String]?, (any Error)?) -> Void)

The list of function names in the model asset.

func modelDescription(completionHandler: (MLModelDescription?, (any Error)?) -> Void)

The default model descripton.

func modelDescription(ofFunctionNamed: String, completionHandler: (MLModelDescription?, (any Error)?) -> Void)

The model descripton for a specified function.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class func load(MLModelAsset, configuration: MLModelConfiguration, completionHandler: (MLModel?, (any Error)?) -> Void)

Construct a model asynchronously from a compiled model asset.

### Model inputs and outputs

Making Predictions with a Sequence of Inputs

Integrate a recurrent neural network model to process sequences of inputs.

class MLFeatureValue

A generic wrapper around an underlying value and the value’s type.

struct MLSendableFeatureValue

A sendable feature value.

protocol MLFeatureProvider

An interface that represents a collection of values for either a model’s input or its output.

class MLDictionaryFeatureProvider

A convenience wrapper for the given dictionary of data.

protocol MLBatchProvider

An interface that represents a collection of feature providers.

class MLArrayBatchProvider

A convenience wrapper for batches of feature providers.

