

- ML Compute
-  MLCMultiheadAttentionLayer Deprecated

Class

# MLCMultiheadAttentionLayer

A multihead, scaled dot-product attention layer that attends to one or more entries in the input key-value pairs.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCMultiheadAttentionLayer
```

## Overview

The dimensions of projections are as follows:

Query  
`(1, headCount, keyDimension/headCount, modelDimension)`

Key  
`(1, headCount, keyDimension/headCount, modelDimension)`

Value  
`(1, headCount, valueDimension/headCount, modelDimension)`

Output  
`(1, 1, modelDimension, valueDimension)`

\`\`

## Topics

### Creating Multi-Head Attention Layers

convenience init?(descriptor: MLCMultiheadAttentionDescriptor, weights: [MLCTensor], biases: [MLCTensor]?, attentionBiases: [MLCTensor]?)

Creates a multi-head attention layer with the descriptor, weights, and biases you specify.

class MLCMultiheadAttentionDescriptor

A configuration object you use to create a multi-head attention layer.

### Inspecting Multi-Head Attention Layers

var descriptor: MLCMultiheadAttentionDescriptor

The configuration object you use to create the multi-head attention layer.

var weights: [MLCTensor]

The array of weights you use for query, key, value, and output projections.

var biases: [MLCTensor]?

The array of biases you use for query, key, value, and output projections.

var attentionBiases: [MLCTensor]?

The array of attention biases you use for key and value.

var weightsParameters: [MLCTensorParameter]

The array of weights tensor parameters you use for optimizer updates.

var biasesParameters: [MLCTensorParameter]?

The array of biases tensor parameters you use for optimizer updates.

## Relationships

### Inherits From

- MLCLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Activation Layers

class MLCActivationLayer

A layer that applies an activation function to the source tensor and produces an output.

Deprecated

class MLCSoftmaxLayer

A layer that outputs a probability distribution as attention weights.

Deprecated

