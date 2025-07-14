

- Core ML
-  MLModelStructure 

Enumeration

# MLModelStructure

An enum representing the structure of a model.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

``` source
enum MLModelStructure
```

## Overview

```
// Load the model structure.
let modelStructure = await try MLModelStructure.load(contentsOf: modelURL)
switch modelStructure {
case .program(let program):
   // Examine ML Program model.
case .neuralNetwork(let neuralNetwork):
   // Examine Neural network model
case .pipeline(let pipeline)
   // Examine Pipeline model
default:
   // The model type is something else.
}
```

## Topics

### Enumeration Cases

case neuralNetwork(MLModelStructure.NeuralNetwork)

case pipeline(MLModelStructure.Pipeline)

case program(MLModelStructure.Program)

case unsupported

### Type Methods

static func load(asset: MLModelAsset) async throws -> MLModelStructure

static func load(contentsOf: URL) async throws -> MLModelStructure

### Structures

struct NeuralNetwork

struct Pipeline

struct Program

## Relationships

### Conforms To

- Sendable

## See Also

### Compute plan

class MLComputePlan

A class representing the compute plan of a model.

struct MLComputePolicy

The compute policy determining what compute device, or compute devices, to execute ML workloads on.

func withMLTensorComputePolicy&lt;R>(MLComputePolicy, () async throws -> R) async rethrows -> R

Calls the given closure within a task-local context using the specified compute policy to influence what compute device tensor operations are executed on.

func withMLTensorComputePolicy&lt;Result>(MLComputePolicy, () throws -> Result) rethrows -> Result

Calls the given closure within a task-local context using the specified compute policy to influence what compute device tensor operations are executed on.

