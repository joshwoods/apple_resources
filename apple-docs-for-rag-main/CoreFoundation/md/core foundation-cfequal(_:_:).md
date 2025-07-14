

- Core Foundation
-  CFEqual(\_:\_:) 

Function

# CFEqual(\_:\_:)

Determines whether two Core Foundation objects are considered equal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFEqual(
    _ cf1: CFTypeRef!,
    _ cf2: CFTypeRef!
) -> Bool
```

## Parameters 

`cf1`  

A CFType object to compare to `cf2`.

`cf2`  

A CFType object to compare to `cf1`.

## Return Value

`true` if `cf1` and `cf2` are of the same type and considered equal, otherwise `false`.

## Discussion

Equality is something specific to each Core Foundation opaque type. For example, two CFNumber objects are equal if the numeric values they represent are equal. Two CFString objects are equal if they represent identical sequences of characters, regardless of encoding.

