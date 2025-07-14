

- Core ML
-  MLArrayBatchProvider 

Class

# MLArrayBatchProvider

A convenience wrapper for batches of feature providers.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class MLArrayBatchProvider
```

## Overview

This batch provider supports an array of feature providers or a dictionary of arrays of feature values.

## Topics

### Initializers

init(array: [any MLFeatureProvider])

Creates the batch provider based on the array of feature providers.

init(dictionary: [String : [Any]]) throws

Creates a batch provider based on feature names and their associated arrays of data.

### Accessing the Feature Providers

var array: [any MLFeatureProvider]

The array of feature providers.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MLBatchProvider
- NSObjectProtocol

## See Also

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

class MLModelAsset

An abstraction of a compiled Core ML model asset.

