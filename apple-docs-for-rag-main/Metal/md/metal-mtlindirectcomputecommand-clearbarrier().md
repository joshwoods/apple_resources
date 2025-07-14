

- Metal
- MTLIndirectComputeCommand
-  clearBarrier() 

Instance Method

# clearBarrier()

Removes any barrier set on the command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
func clearBarrier()
```

**Required**

## Discussion

You must set or clear barriers (as needed) before executing any of the commands in the indirect command buffer.

## See Also

### Synchronizing Command Execution

func setBarrier()

Adds a barrier to ensure that commands executed prior to this command are complete before this command executes.

**Required**

