

- Metal
- MTLIndirectCommandBuffer
-  indirectComputeCommand(at:) 

Instance Method

# indirectComputeCommand(at:)

Gets the compute command at the given index.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedtvOS 13.0–14.0DeprecatedvisionOS

``` source
func indirectComputeCommand(at Index: Int) -> any MTLIndirectComputeCommand
```

## Parameters 

`Index`  

The index of the command to retrieve.

## Discussion

Call this method only if the indirect command buffer contains compute commands.

## See Also

### Retrieving Commands

func indirectRenderCommandAt(Int) -> any MTLIndirectRenderCommand

Gets the render command at the given index.

**Required**

func indirectComputeCommandAt(Int) -> any MTLIndirectComputeCommand

Gets the compute command at the given index.

**Required**

