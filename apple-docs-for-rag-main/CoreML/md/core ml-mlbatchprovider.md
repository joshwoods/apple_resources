

- Core ML
-  MLBatchProvider 

Protocol

# MLBatchProvider

An interface that represents a collection of feature providers.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
protocol MLBatchProvider
```

## Overview

Similar to the MLFeatureProvider, this interface allows you to define your own batch provider. If you collect your data asynchronously or it is memory intensive, implement this protocol on your data structure to optimize performance with batch processing.

## Topics

### Accessing Values

func features(at: Int) -> any MLFeatureProvider

Returns the feature provider at the given index.

**Required**

var count: Int

The number of feature providers in this batch.

**Required**

## Relationships

### Conforming Types

- MLArrayBatchProvider

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

class MLArrayBatchProvider

A convenience wrapper for batches of feature providers.

class MLModelAsset

An abstraction of a compiled Core ML model asset.

