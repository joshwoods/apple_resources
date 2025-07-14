

- Core ML
-  MLModelConfiguration 

Class

# MLModelConfiguration

The settings for creating or updating a machine learning model.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class MLModelConfiguration
```

## Overview

Use a model configuration to:

- Set or override model parameters.

- Designate which device the model uses to make predictions, such as a GPU.

- Restrict the model to use a specific computational device category, such as a CPU.

You typically use a model configuration instance to configure an MLModel instance as you create it with init(contentsOf:configuration:) or create an MLUpdateTask. See Personalizing a Model with On-Device Updates.

Configure your model parameters by setting values for each relevant MLParameterKey in the parameters property.

## Topics

### Configuring Model Parameters

var modelDisplayName: String?

A human readable name of a model for display purposes.

var parameters: [MLParameterKey : Any]?

A dictionary of configuration settings your app can override when loading a model.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

### Configuring GPU Usage

var preferredMetalDevice: (any MTLDevice)?

The metal device you prefer this model use to make predictions (inference) and update the model.

var allowLowPrecisionAccumulationOnGPU: Bool

A Boolean value that determines whether to allow low-precision accumulation on a GPU.

### Allowing Access to Processing Units

var computeUnits: MLComputeUnits

The processing unit or units the model uses to make predictions.

enum MLComputeUnits

The set of processing-unit configurations the model can use to make predictions.

### Instance Properties

var optimizationHints: MLOptimizationHints

var functionName: String?

Function name that `MLModel` will use.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Supporting Types

struct MLOptimizationHints

class MLKey

An abstract base class for machine learning key types.

