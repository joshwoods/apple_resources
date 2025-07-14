

- Core Foundation
-  CFFileDescriptorGetNativeDescriptor(\_:) 

Function

# CFFileDescriptorGetNativeDescriptor(\_:)

Returns the native file descriptor for a given CFFileDescriptor.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileDescriptorGetNativeDescriptor(_ f: CFFileDescriptor!) -> CFFileDescriptorNativeDescriptor
```

## Parameters 

`f`  

A CFFileDescriptor.

## Return Value

The native file descriptor for `f`.

## See Also

### Related Documentation

func CFFileDescriptorInvalidate(CFFileDescriptor!)

Invalidates a CFFileDescriptor object.

### Getting Information About a File Descriptor

func CFFileDescriptorIsValid(CFFileDescriptor!) -> Bool

Returns a Boolean value that indicates whether the native file descriptor for a given CFFileDescriptor is valid.

func CFFileDescriptorGetContext(CFFileDescriptor!, UnsafeMutablePointer&lt;CFFileDescriptorContext>!)

Gets the context for a given CFFileDescriptor.

