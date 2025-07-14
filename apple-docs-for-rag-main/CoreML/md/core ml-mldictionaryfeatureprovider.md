

- Core ML
-  MLDictionaryFeatureProvider 

Class

# MLDictionaryFeatureProvider

A convenience wrapper for the given dictionary of data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class MLDictionaryFeatureProvider
```

## Overview

If your input data is stored in a dictionary, consider this type of MLFeatureProvider that is backed by a dictionary. It is a convenience interface, saving you the trouble of iterating through the dictionary to assign all of its values.

## Topics

### Creating the Provider

init(dictionary: [String : Any]) throws

Creates the feature provider based on a dictionary.

### Accessing the Features

subscript(String) -> MLFeatureValue?

Subscript interface for the feature provider to pass through to the dictionary.

var dictionary: [String : MLFeatureValue]

The backing dictionary.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MLFeatureProvider
- NSCoding
- NSFastEnumeration
- NSObjectProtocol
- NSSecureCoding

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

protocol MLBatchProvider

An interface that represents a collection of feature providers.

class MLArrayBatchProvider

A convenience wrapper for batches of feature providers.

class MLModelAsset

An abstraction of a compiled Core ML model asset.

