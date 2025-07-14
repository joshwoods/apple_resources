

- Core Foundation
-  CFFileDescriptorCreate(\_:\_:\_:\_:\_:) 

Function

# CFFileDescriptorCreate(\_:\_:\_:\_:\_:)

Creates a new CFFileDescriptor.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileDescriptorCreate(
    _ allocator: CFAllocator!,
    _ fd: CFFileDescriptorNativeDescriptor,
    _ closeOnInvalidate: Bool,
    _ callout: CFFileDescriptorCallBack!,
    _ context: UnsafePointer!
) -> CFFileDescriptor!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new file descriptor object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`fd`  

The file descriptor for the new CFFileDescriptor.

`closeOnInvalidate`  

`true` if the new CFFileDescriptor should close `fd` when it is invalidated, otherwise `false`.

`callout`  

The CFFileDescriptorCallBack for the new CFFileDescriptor.

`context`  

Contextual information for the new CFFileDescriptor.

## Return Value

A new CFFileDescriptor or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Related Documentation

func CFFileDescriptorGetContext(CFFileDescriptor!, UnsafeMutablePointer&lt;CFFileDescriptorContext>!)

Gets the context for a given CFFileDescriptor.

func CFFileDescriptorInvalidate(CFFileDescriptor!)

Invalidates a CFFileDescriptor object.

