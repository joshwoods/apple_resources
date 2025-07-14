

- Metal
- MTLBlitCommandEncoder
-  updateFence(\_:) 

Instance Method

# updateFence(\_:)

Encodes a command that instructs the GPU to update a fence, which signals passes waiting on the fence.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func updateFence(_ fence: any MTLFence)
```

**Required**

## Parameters 

`fence`  

An MTLFence instance to update.

## Discussion

Fences maintain order to prevent GPU data hazards as the GPU runs various passes within the same command queue. Metal evaluates fences and the commands that depend on them when your app commits the enclosing MTLCommandBuffer.

Important

For a pass that updates and waits for the same fence, call waitForFence(_:) before you call updateFence(_:). Updating a fence before waiting on it within the same encoder can cause GPU deadlock.

## See Also

### Working with Fences

func waitForFence(any MTLFence)

Encodes a command that instructs the GPU to wait until a pass updates a fence.

**Required**

