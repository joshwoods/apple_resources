

- Core Foundation
-  CFRangeMake(\_:\_:) 

Function

# CFRangeMake(\_:\_:)

Declares and initializes a `CFRange` structure.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRangeMake(
    _ loc: CFIndex,
    _ len: CFIndex
) -> CFRange
```

## Parameters 

`loc`  

The starting location of the range.

`len`  

The length of the range.

## Return Value

An initialized structure of type CFRange.

## Discussion

This is an in-line convenience function for creating initialized CFRange structures.

