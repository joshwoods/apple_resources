

- Metal
- MTLResourceStateCommandEncoder
-  wait(for:) 

Instance Method

# wait(for:)

Encodes a command that instructs the GPU to pause before starting the resource state commands until another pass updates a fence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

**Mac Catalyst, macOS**

``` source
optional func wait(for fence: any MTLFence)
```

**iOS, iPadOS, tvOS, visionOS**

``` source
func wait(for fence: any MTLFence)
```

**Required**

## Parameters 

`fence`  

An MTLFence instance to pause execution on until updated.

## Discussion

Fences maintain order to prevent GPU data hazards as the GPU runs various passes within the same command queue. The encoded resource state commands wait for a pass to update `fence` before running.

The GPU driver evaluates the pass’s fences and the commands that depend on them when your app commits the enclosing MTLCommandBuffer.

## See Also

### Performing Fence Operations

func update(any MTLFence)

Encodes a command that instructs the GPU to update a fence, which signals passes waiting on the fence.

**Required**

