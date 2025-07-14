

- Foundation
- MachError
-  memoryRestartCopy 

Type Property

# memoryRestartCopy

A strategic copy was attempted of an object upon which a quicker copy is now possible. The caller should retry the copy using vm_object_copy_quickly. This error code is seen only by the kernel.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var memoryRestartCopy: MachError.Code { get }
```

