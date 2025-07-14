

- Metal
- MTLCommandBuffer
-  retainedReferences 

Instance Property

# retainedReferences

A Boolean value that indicates whether the command buffer maintains strong references to the resources it uses.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var retainedReferences: Bool { get }
```

**Required**

## Discussion

You can configure this property when you create a command buffer by setting retainedReferences of an MTLCommandBufferDescriptor instance and calling the makeCommandBuffer(descriptor:) method. The makeCommandBuffer() method sets this property to true, and makeCommandBufferWithUnretainedReferences() sets it to false.

If false, your app is responsible for maintaining strong references to all the resources the command buffer relies on until it completes.

Important

Releasing a resource before a command buffer’s commands complete may cause a runtime error or erratic behavior.

