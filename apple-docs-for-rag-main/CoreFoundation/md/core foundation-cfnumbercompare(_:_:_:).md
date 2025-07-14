

- Core Foundation
-  CFNumberCompare(\_:\_:\_:) 

Function

# CFNumberCompare(\_:\_:\_:)

Compares two CFNumber objects and returns a comparison result.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberCompare(
    _ number: CFNumber!,
    _ otherNumber: CFNumber!,
    _ context: UnsafeMutableRawPointer!
) -> CFComparisonResult
```

## Parameters 

`number`  

The first CFNumber object to compare.

`otherNumber`  

The second CFNumber object to compare.

`context`  

Pass `NULL`.

## Return Value

A CFComparisonResult constant that indicates whether `number` is equal to, less than, or greater than `otherNumber`.

## Discussion

When comparing two CFNumber objects using this function, one or both objects can represent a special-case number such as signed 0, signed infinity, or NaN.

The following rules apply:

- Negative 0 compares less than positive 0.

- Positive infinity compares greater than everything except itself, to which it compares equal.

- Negative infinity compares less than everything except itself, to which it compares equal.

- If both numbers are NaN, then they compare equal.

- If only one of the numbers is NaN, then the NaN compares greater than the other number if it is negative, and smaller than the other number if it is positive.

