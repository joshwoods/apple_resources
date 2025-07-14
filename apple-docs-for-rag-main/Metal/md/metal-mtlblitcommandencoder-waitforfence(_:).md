

- Metal
- MTLBlitCommandEncoder
-  waitForFence(\_:) 

Instance Method

# waitForFence(\_:)

Encodes a command that instructs the GPU to wait until a pass updates a fence.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func waitForFence(_ fence: any MTLFence)
```

**Required**

## Parameters 

`fence`  

An MTLFence instance the GPU waits for before running this blit pass.

## Discussion

Fences maintain order to prevent GPU data hazards as the GPU runs various passes within the same command queue. The GPU driver evaluates the fences and the commands that depend on them when your app commits the enclosing MTLCommandBuffer.

Important

For a blit pass that updates and waits for the same fence, you can only call waitForFence(_:) before you call updateFence(_:). Updating a fence before waiting on it within the same encoder can cause GPU deadlock.

The GPU driver evaluates the pass’s fences and the commands that depend on them when your app commits the enclosing MTLCommandBuffer.

## See Also

### Working with Fences

func updateFence(any MTLFence)

Encodes a command that instructs the GPU to update a fence, which signals passes waiting on the fence.

**Required**

