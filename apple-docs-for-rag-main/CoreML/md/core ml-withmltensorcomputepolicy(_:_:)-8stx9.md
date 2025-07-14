

- Core ML
-  withMLTensorComputePolicy(\_:\_:) 

Function

# withMLTensorComputePolicy(\_:\_:)

Calls the given closure within a task-local context using the specified compute policy to influence what compute device tensor operations are executed on.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func withMLTensorComputePolicy(
    _ computePolicy: MLComputePolicy,
    _ body: () async throws -> R
) async rethrows -> R
```

## Parameters 

`computePolicy`  

A compute policy that will be set before the closure gets called and restored after the closure returns.

`body`  

A nullary closure. If the closure has a return value, that value is also used as the return value of the `withMLTensorComputePolicy(_:_:)` function.

## Return Value

The return value, if any, of the `body` closure.

## See Also

### Compute plan

class MLComputePlan

A class representing the compute plan of a model.

enum MLModelStructure

An enum representing the structure of a model.

struct MLComputePolicy

The compute policy determining what compute device, or compute devices, to execute ML workloads on.

func withMLTensorComputePolicy&lt;Result>(MLComputePolicy, () throws -> Result) rethrows -> Result

Calls the given closure within a task-local context using the specified compute policy to influence what compute device tensor operations are executed on.

