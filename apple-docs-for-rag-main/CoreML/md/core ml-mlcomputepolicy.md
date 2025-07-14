

- Core ML
-  MLComputePolicy 

Structure

# MLComputePolicy

The compute policy determining what compute device, or compute devices, to execute ML workloads on.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MLComputePolicy
```

## Topics

### Initializers

init(MLComputeUnits)

Creates a new compute policy using the given compute units.

### Type Properties

static var cpuAndGPU: MLComputePolicy

Execute ML workloads using the GPU if available, otherwise falling back to the CPU.

static var cpuOnly: MLComputePolicy

Execute ML workloads using the CPU.

### Default Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Compute plan

class MLComputePlan

A class representing the compute plan of a model.

enum MLModelStructure

An enum representing the structure of a model.

func withMLTensorComputePolicy&lt;R>(MLComputePolicy, () async throws -> R) async rethrows -> R

Calls the given closure within a task-local context using the specified compute policy to influence what compute device tensor operations are executed on.

func withMLTensorComputePolicy&lt;Result>(MLComputePolicy, () throws -> Result) rethrows -> Result

Calls the given closure within a task-local context using the specified compute policy to influence what compute device tensor operations are executed on.

