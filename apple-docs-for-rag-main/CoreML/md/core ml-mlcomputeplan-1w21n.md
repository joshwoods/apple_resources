

- Core ML
-  MLComputePlan 

Class

# MLComputePlan

A class representing the compute plan of a model.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

``` source
class MLComputePlan
```

## Overview

The application can use the compute plan to estimate the necessary cost and resources of the model before running the predictions.

```
// Load the compute plan of an ML Program model.
let computePlan = try await MLComputePlan.load(contentsOf: modelURL, configuration: configuration)
guard case let .program(program) = computePlan.modelStructure else {
   fatalError("Unexpected model type.")
}
 // Get the main function.
guard let mainFunction = program.functions["main"] else {
   fatalError("Missing main function.")
}

let operations = mainFunction.block.operations
for operation in operations {
   // Get the compute device usage for the operation.
   let computeDeviceUsage = computePlan.deviceUsage(for: operation)
   // Get the estimated cost of executing the operation.
   let estimatedCost = computePlan.estimatedCost(of: operation)
}
```

## Topics

### Instance Properties

let modelStructure: MLModelStructure

modelStructure

### Instance Methods

func deviceUsage(for: MLModelStructure.NeuralNetwork.Layer) -> MLComputePlan.DeviceUsage?

func deviceUsage(for: MLModelStructure.Program.Operation) -> MLComputePlan.DeviceUsage?

func estimatedCost(of: MLModelStructure.Program.Operation) -> MLComputePlan.Cost?

- computeDeviceUsageForMLProgramOperation:

- computeDeviceUsageForNeuralNetworkLayer:

- estimatedCostOfMLProgramOperation:

### Type Methods

static func load(asset: MLModelAsset, configuration: MLModelConfiguration) async throws -> MLComputePlan

static func load(contentsOf: URL, configuration: MLModelConfiguration) async throws -> MLComputePlan

### Structures

struct Cost

struct DeviceUsage

+ loadContentsOfURL:configuration:completionHandler:

+ loadModelAsset:configuration:completionHandler:

## See Also

### Compute plan

enum MLModelStructure

An enum representing the structure of a model.

struct MLComputePolicy

The compute policy determining what compute device, or compute devices, to execute ML workloads on.

func withMLTensorComputePolicy&lt;R>(MLComputePolicy, () async throws -> R) async rethrows -> R

Calls the given closure within a task-local context using the specified compute policy to influence what compute device tensor operations are executed on.

func withMLTensorComputePolicy&lt;Result>(MLComputePolicy, () throws -> Result) rethrows -> Result

Calls the given closure within a task-local context using the specified compute policy to influence what compute device tensor operations are executed on.

