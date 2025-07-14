

- Core Foundation
-  CFFileDescriptorGetContext(\_:\_:) 

Function

# CFFileDescriptorGetContext(\_:\_:)

Gets the context for a given CFFileDescriptor.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileDescriptorGetContext(
    _ f: CFFileDescriptor!,
    _ context: UnsafeMutablePointer!
)
```

## Parameters 

`f`  

A CFFileDescriptor.

`context`  

Upon return, contains the context passed to `f` in CFFileDescriptorCreate(_:_:_:_:_:).

## See Also

### Related Documentation

func CFFileDescriptorCreate(CFAllocator!, CFFileDescriptorNativeDescriptor, Bool, CFFileDescriptorCallBack!, UnsafePointer&lt;CFFileDescriptorContext>!) -> CFFileDescriptor!

Creates a new CFFileDescriptor.

### Getting Information About a File Descriptor

func CFFileDescriptorGetNativeDescriptor(CFFileDescriptor!) -> CFFileDescriptorNativeDescriptor

Returns the native file descriptor for a given CFFileDescriptor.

func CFFileDescriptorIsValid(CFFileDescriptor!) -> Bool

Returns a Boolean value that indicates whether the native file descriptor for a given CFFileDescriptor is valid.

