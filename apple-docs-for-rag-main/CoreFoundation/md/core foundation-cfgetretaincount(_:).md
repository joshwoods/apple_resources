

- Core Foundation
-  CFGetRetainCount(\_:) 

Function

# CFGetRetainCount(\_:)

Returns the reference count of a Core Foundation object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFGetRetainCount(_ cf: CFTypeRef!) -> CFIndex
```

## Parameters 

`cf`  

The CFType object to examine.

## Return Value

A number representing the reference count of `cf`.

## Discussion

You increment the reference count using the CFRetain function, and decrement the reference count using the CFRelease function.

This function may be useful for debugging memory leaks. You normally do not use this function, otherwise.

## See Also

### Memory Management

func CFGetAllocator(CFTypeRef!) -> CFAllocator!

Returns the allocator used to allocate a Core Foundation object.

