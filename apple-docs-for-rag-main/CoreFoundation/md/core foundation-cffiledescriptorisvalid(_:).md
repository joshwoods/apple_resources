

- Core Foundation
-  CFFileDescriptorIsValid(\_:) 

Function

# CFFileDescriptorIsValid(\_:)

Returns a Boolean value that indicates whether the native file descriptor for a given CFFileDescriptor is valid.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileDescriptorIsValid(_ f: CFFileDescriptor!) -> Bool
```

## Parameters 

`f`  

A CFFileDescriptor.

## Return Value

`true` if the native file descriptor for `f` is valid, otherwise `false`.

## See Also

### Related Documentation

func CFFileDescriptorInvalidate(CFFileDescriptor!)

Invalidates a CFFileDescriptor object.

### Getting Information About a File Descriptor

func CFFileDescriptorGetNativeDescriptor(CFFileDescriptor!) -> CFFileDescriptorNativeDescriptor

Returns the native file descriptor for a given CFFileDescriptor.

func CFFileDescriptorGetContext(CFFileDescriptor!, UnsafeMutablePointer&lt;CFFileDescriptorContext>!)

Gets the context for a given CFFileDescriptor.

