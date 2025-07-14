

- Core Foundation
-  CFCharacterSetCreateMutableCopy(\_:\_:) 

Function

# CFCharacterSetCreateMutableCopy(\_:\_:)

Creates a new mutable character set with the values from another character set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFCharacterSetCreateMutableCopy(
    _ alloc: CFAllocator!,
    _ theSet: CFCharacterSet!
) -> CFMutableCharacterSet!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theSet`  

The character set to copy.

## Return Value

A new mutable character set containing the same characters as `theSet`. Ownership follows the The Create Rule.

## See Also

### Creating a Mutable Character Set

func CFCharacterSetCreateMutable(CFAllocator!) -> CFMutableCharacterSet!

Creates a new empty mutable character set.

