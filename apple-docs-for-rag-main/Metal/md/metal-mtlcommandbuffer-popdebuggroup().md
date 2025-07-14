

- Metal
- MTLCommandBuffer
-  popDebugGroup() 

Instance Method

# popDebugGroup()

Marks the end of a debug group and, if applicable, restores the previous group from a stack.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func popDebugGroup()
```

**Required**

## Discussion

Use pushDebugGroup(_:) to group commands within the command buffer, which adds a new group to a stack, effectively nesting a group within any previous group. Call popDebugGroup() to mark the end of a group of commands within the command buffer, and restore the previous group, if applicable. You can inspect the group and the commands it contains when viewing the contents of a frame capture with Metal Debugger.

Labels can help you profile and debug your app at runtime with Metal Debugger and other tools. See `Enhancing Frame Capture by Using Labels` for more information about using labels and other debugging techniques.

## See Also

### Grouping Commands within a GPU Frame Capture

func pushDebugGroup(String)

Marks the beginning of a debug group and gives it an identifying label, which temporarily replaces the previous group, if applicable.

**Required**

