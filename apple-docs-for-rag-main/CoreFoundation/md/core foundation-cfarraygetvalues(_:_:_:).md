

- Core Foundation
-  CFArrayGetValues(\_:\_:\_:) 

Function

# CFArrayGetValues(\_:\_:\_:)

Fills a buffer with values from an array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayGetValues(
    _ theArray: CFArray!,
    _ range: CFRange,
    _ values: UnsafeMutablePointer!
)
```

## Parameters 

`theArray`  

The array to examine.

`range`  

The range of values within `theArray` to retrieve. The range must lie within the bounds of `theArray`. The range may be empty (length `0`), in which case no values are put into the buffer `values`.

`values`  

A C array of pointer-sized values to be filled with values from `theArray`. The values in the C array are in the same order as they appear in `theArray`. If this value is not a valid pointer to a C array of at least `range.length` pointers, the behavior is undefined. If the values are Core Foundation objects, ownership follows The Get Rule.

## See Also

### Examining an Array

func CFArrayBSearchValues(CFArray!, CFRange, UnsafeRawPointer!, CFComparatorFunction!, UnsafeMutableRawPointer!) -> CFIndex

Searches an array for a value using a binary search algorithm.

func CFArrayContainsValue(CFArray!, CFRange, UnsafeRawPointer!) -> Bool

Reports whether or not a value is in an array.

func CFArrayGetCount(CFArray!) -> CFIndex

Returns the number of values currently in an array.

func CFArrayGetCountOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Counts the number of times a given value occurs in an array.

func CFArrayGetFirstIndexOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Searches an array forward for a value.

func CFArrayGetLastIndexOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Searches an array backward for a value.

func CFArrayGetValueAtIndex(CFArray!, CFIndex) -> UnsafeRawPointer!

Retrieves a value at a given index.

