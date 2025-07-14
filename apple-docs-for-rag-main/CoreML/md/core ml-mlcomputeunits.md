

- Core ML
-  MLComputeUnits 

Enumeration

# MLComputeUnits

The set of processing-unit configurations the model can use to make predictions.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum MLComputeUnits
```

## Overview

Use this enumeration to set or inspect the processing units you allow a model to use when it makes a prediction.

Use `all` to allow the OS to select the best processing unit to use (including the neural engine, if available).

Use MLComputeUnits.cpuOnly to restrict the model to the CPU, if your app might run in the background or runs other GPU intensive tasks.

## Topics

### Processing Unit Configurations

case all

The option you choose to allow the model to use all compute units available, including the neural engine.

case cpuOnly

The option you choose to limit the model to only use the CPU.

case cpuAndGPU

The option you choose to allow the model to use both the CPU and GPU, but not the neural engine.

case cpuAndNeuralEngine

The option you choose to allow the model to use both the CPU and neural engine, but not the GPU.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Allowing Access to Processing Units

var computeUnits: MLComputeUnits

The processing unit or units the model uses to make predictions.

