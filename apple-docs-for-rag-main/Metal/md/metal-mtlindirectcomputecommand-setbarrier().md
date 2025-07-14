

- Metal
- MTLIndirectComputeCommand
-  setBarrier() 

Instance Method

# setBarrier()

Adds a barrier to ensure that commands executed prior to this command are complete before this command executes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
func setBarrier()
```

**Required**

## Discussion

Set or clear barriers (as needed) before encoding the command.

## See Also

### Synchronizing Command Execution

func clearBarrier()

Removes any barrier set on the command.

**Required**

