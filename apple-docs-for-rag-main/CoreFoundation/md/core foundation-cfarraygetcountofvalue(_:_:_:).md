

- Core Foundation
-  CFArrayGetCountOfValue(\_:\_:\_:) 

Function

# CFArrayGetCountOfValue(\_:\_:\_:)

Counts the number of times a given value occurs in an array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayGetCountOfValue(
    _ theArray: CFArray!,
    _ range: CFRange,
    _ value: UnsafeRawPointer!
) -> CFIndex
```

## Parameters 

`theArray`  

The array to examine.

`range`  

The range within `theArray` to search. The range must lie within the bounds of `theArray`). The range may be empty (length `0`).

`value`  

The value for which to find matches in `theArray`. The equal callback provided when `theArray` was created is used to compare. If the equal callback was `NULL`, pointer equality (in C, `==`) is used. If `value`, or any other value in `theArray`, is not understood by the equal callback, the behavior is undefined.

## Return Value

The number of times `value` occurs in `theArray`, within the specified range.

## See Also

### Examining an Array

func CFArrayBSearchValues(CFArray!, CFRange, UnsafeRawPointer!, CFComparatorFunction!, UnsafeMutableRawPointer!) -> CFIndex

Searches an array for a value using a binary search algorithm.

func CFArrayContainsValue(CFArray!, CFRange, UnsafeRawPointer!) -> Bool

Reports whether or not a value is in an array.

func CFArrayGetCount(CFArray!) -> CFIndex

Returns the number of values currently in an array.

func CFArrayGetFirstIndexOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Searches an array forward for a value.

func CFArrayGetLastIndexOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Searches an array backward for a value.

func CFArrayGetValues(CFArray!, CFRange, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from an array.

func CFArrayGetValueAtIndex(CFArray!, CFIndex) -> UnsafeRawPointer!

Retrieves a value at a given index.

