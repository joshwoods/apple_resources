

- Core Foundation
-  CFArrayGetFirstIndexOfValue(\_:\_:\_:) 

Function

# CFArrayGetFirstIndexOfValue(\_:\_:\_:)

Searches an array forward for a value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayGetFirstIndexOfValue(
    _ theArray: CFArray!,
    _ range: CFRange,
    _ value: UnsafeRawPointer!
) -> CFIndex
```

## Parameters 

`theArray`  

The array to examine.

`range`  

The range within `theArray` to search. The range must lie within the bounds of `theArray`. The range may be empty (length `0`). The search progresses from the lowest index defined by the range to the highest.

`value`  

The value for which to find a match in `theArray`. The equal callback provided when `theArray` was created is used to compare. If the equal callback was `NULL`, pointer equality (in C, ==) is used. If `value`, or any other value in `theArray`, is not understood by the equal callback, the behavior is undefined.

## Return Value

The lowest index of the matching values in the range, or `-1` if no value in the range matched.

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

func CFArrayGetLastIndexOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Searches an array backward for a value.

func CFArrayGetValues(CFArray!, CFRange, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from an array.

func CFArrayGetValueAtIndex(CFArray!, CFIndex) -> UnsafeRawPointer!

Retrieves a value at a given index.

