

- Core Foundation
-  CFAttributedStringCreateMutable(\_:\_:) 

Function

# CFAttributedStringCreateMutable(\_:\_:)

Creates a mutable attributed string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringCreateMutable(
    _ alloc: CFAllocator!,
    _ maxLength: CFIndex
) -> CFMutableAttributedString!
```

## Parameters 

`alloc`  

An allocator to be used to allocate memory for the new attributed string. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`maxLength`  

The limit on the length of the new attributed string. The string starts empty and can grow to this length (it can be shorter).

Pass `0` to specify that the maximum length is not limited. The value must not be negative.

## Return Value

A new mutable attributed string. Ownership follows the The Create Rule.

## See Also

### Creating a CFMutableAttributedString

func CFAttributedStringCreateMutableCopy(CFAllocator!, CFIndex, CFAttributedString!) -> CFMutableAttributedString!

Creates a mutable copy of an attributed string.

