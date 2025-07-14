

- Core Foundation
-  CFFileDescriptorInvalidate(\_:) 

Function

# CFFileDescriptorInvalidate(\_:)

Invalidates a CFFileDescriptor object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFFileDescriptorInvalidate(_ f: CFFileDescriptor!)
```

## Parameters 

`f`  

A CFFileDescriptor.

## Discussion

Once invalidated, the CFFileDescriptor object will no longer be read from or written to at the Core Fundation level.

If you passed `true` for the `closeOnInvalidate` parameter when you called CFFileDescriptorCreate(_:_:_:_:_:), this function also closes the underlying file descriptor. If you passed `false`, you must close the descriptor yourself *after* invalidating the CFFileDescriptor object.

Important

You must invalidate the CFFileDescriptor before closing the underlying file descriptor.

## See Also

### Related Documentation

func CFFileDescriptorGetNativeDescriptor(CFFileDescriptor!) -> CFFileDescriptorNativeDescriptor

Returns the native file descriptor for a given CFFileDescriptor.

func CFFileDescriptorIsValid(CFFileDescriptor!) -> Bool

Returns a Boolean value that indicates whether the native file descriptor for a given CFFileDescriptor is valid.

