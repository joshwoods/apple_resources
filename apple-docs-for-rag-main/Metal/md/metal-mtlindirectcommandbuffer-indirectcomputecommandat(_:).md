

- Metal
- MTLIndirectCommandBuffer
-  indirectComputeCommandAt(\_:) 

Instance Method

# indirectComputeCommandAt(\_:)

Gets the compute command at the given index.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
func indirectComputeCommandAt(_ commandIndex: Int) -> any MTLIndirectComputeCommand
```

**Required**

## Parameters 

`commandIndex`  

The index of the command to retrieve.

## Discussion

Call this method only if the indirect command buffer contains compute commands.

## See Also

### Retrieving Commands

func indirectRenderCommandAt(Int) -> any MTLIndirectRenderCommand

Gets the render command at the given index.

**Required**

func indirectComputeCommand(at: Int) -> any MTLIndirectComputeCommand

Gets the compute command at the given index.

