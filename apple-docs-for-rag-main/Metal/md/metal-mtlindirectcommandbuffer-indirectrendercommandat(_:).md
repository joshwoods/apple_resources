

- Metal
- MTLIndirectCommandBuffer
-  indirectRenderCommandAt(\_:) 

Instance Method

# indirectRenderCommandAt(\_:)

Gets the render command at the given index.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func indirectRenderCommandAt(_ commandIndex: Int) -> any MTLIndirectRenderCommand
```

**Required**

## Parameters 

`commandIndex`  

The index of the command to retrieve.

## Discussion

Call this method only if the indirect command buffer contains rendering commands.

## See Also

### Retrieving Commands

func indirectComputeCommandAt(Int) -> any MTLIndirectComputeCommand

Gets the compute command at the given index.

**Required**

func indirectComputeCommand(at: Int) -> any MTLIndirectComputeCommand

Gets the compute command at the given index.

