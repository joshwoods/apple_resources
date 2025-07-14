

- Core Foundation
-  CFAttributedStringCreateMutableCopy(\_:\_:\_:) 

Function

# CFAttributedStringCreateMutableCopy(\_:\_:\_:)

Creates a mutable copy of an attributed string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringCreateMutableCopy(
    _ alloc: CFAllocator!,
    _ maxLength: CFIndex,
    _ aStr: CFAttributedString!
) -> CFMutableAttributedString!
```

## Parameters 

`alloc`  

The allocator to be used to allocate memory for the new attributed string. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`maxLength`  

The limit on the length of the new attributed string. The string starts empty and can grow to this length (it can be shorter).

Pass `0` to specify that the maximum length is not limited. If non-`0`, `maxLength` must be greater than or equal to the length of `aStr`.

`aStr`  

The attributed string to copy.

## Return Value

A mutable copy of `aStr`. Ownership follows the The Create Rule.

## See Also

### Creating a CFMutableAttributedString

func CFAttributedStringCreateMutable(CFAllocator!, CFIndex) -> CFMutableAttributedString!

Creates a mutable attributed string.

