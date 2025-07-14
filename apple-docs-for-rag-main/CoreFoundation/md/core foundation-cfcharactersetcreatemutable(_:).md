

- Core Foundation
-  CFCharacterSetCreateMutable(\_:) 

Function

# CFCharacterSetCreateMutable(\_:)

Creates a new empty mutable character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetCreateMutable(_ alloc: CFAllocator!) -> CFMutableCharacterSet!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

## Return Value

A new empty mutable character set. Ownership follows the The Create Rule.

## See Also

### Creating a Mutable Character Set

func CFCharacterSetCreateMutableCopy(CFAllocator!, CFCharacterSet!) -> CFMutableCharacterSet!

Creates a new mutable character set with the values from another character set.

