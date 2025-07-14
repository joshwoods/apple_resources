

- Metal
- MTLIOCommandBuffer
-  popDebugGroup() 

Instance Method

# popDebugGroup()

Restores the previous name for this input/output command encoder by removing the top item of the debug name stack.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func popDebugGroup()
```

**Required**

## See Also

### Debugging a Command Buffer

var label: String?

An optional name for the input/output command buffer.

**Required**

func pushDebugGroup(String)

Sets the current name for this input/output command encoder by adding it to the top of the debug name stack.

**Required**

