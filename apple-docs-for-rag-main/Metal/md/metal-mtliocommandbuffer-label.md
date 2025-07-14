

- Metal
- MTLIOCommandBuffer
-  label 

Instance Property

# label

An optional name for the input/output command buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var label: String? { get set }
```

**Required**

## See Also

### Debugging a Command Buffer

func pushDebugGroup(String)

Sets the current name for this input/output command encoder by adding it to the top of the debug name stack.

**Required**

func popDebugGroup()

Restores the previous name for this input/output command encoder by removing the top item of the debug name stack.

**Required**

