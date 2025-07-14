

- Core Foundation
-  CFFileDescriptorCreateRunLoopSource(\_:\_:\_:) 

Function

# CFFileDescriptorCreateRunLoopSource(\_:\_:\_:)

Creates a new runloop source for a given CFFileDescriptor.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileDescriptorCreateRunLoopSource(
    _ allocator: CFAllocator!,
    _ f: CFFileDescriptor!,
    _ order: CFIndex
) -> CFRunLoopSource!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new bag and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`f`  

A CFFileDescriptor.

`order`  

The order for the new run loop (see CFRunLoopSourceCreate(_:_:_:)).

## Return Value

A new runloop source for `f`, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

The context for the new runloop (see CFRunLoopSourceCreate(_:_:_:)) is the same as the context passed in when the CFFileDescriptor was created (see CFFileDescriptorCreate(_:_:_:_:_:)).

