

- FSKit
- FSVolume
- FSVolume.AccessMask
-  formUnion(\_:) 

Instance Method

# formUnion(\_:)

Inserts the elements of another set into this option set.

FSKitSwiftmacOS 15.4+

``` source
mutating func formUnion(_ other: Self)
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Parameters 

`other`  

An option set.

## Discussion

This method is implemented as a `|` (bitwise OR) operation on the two sets’ raw values.

