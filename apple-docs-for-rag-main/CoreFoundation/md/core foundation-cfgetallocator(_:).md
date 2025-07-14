

- Core Foundation
-  CFGetAllocator(\_:) 

Function

# CFGetAllocator(\_:)

Returns the allocator used to allocate a Core Foundation object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFGetAllocator(_ cf: CFTypeRef!) -> CFAllocator!
```

## Parameters 

`cf`  

The CFType object to examine.

## Return Value

The allocator used to allocate memory for `cf`.

## Discussion

When you are creating a Core Foundation object sometimes you want to ensure that the block of memory allocated for the object is from the same allocator used for another object. One way to do this is to reuse the allocator assigned to an existing Core Foundation object when you call a “creation” function.

## See Also

### Memory Management

func CFGetRetainCount(CFTypeRef!) -> CFIndex

Returns the reference count of a Core Foundation object.

