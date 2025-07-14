

- Core Foundation
-  CFArrayContainsValue(\_:\_:\_:) 

Function

# CFArrayContainsValue(\_:\_:\_:)

Reports whether or not a value is in an array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayContainsValue(
    _ theArray: CFArray!,
    _ range: CFRange,
    _ value: UnsafeRawPointer!
) -> Bool
```

## Parameters 

`theArray`  

The array to search.

`range`  

The range within `theArray` to search. The range must not exceed the bounds of `theArray`). The range may be empty (length `0`).

`value`  

The value to match in `theArray`. The equal callback provided when `theArray` was created is used to compare. If the equal callback was `NULL`, pointer equality (in C, ==) is used. If `value`, or any other value in `theArray`, is not understood by the equal callback, the behavior is undefined.

## Return Value

`true`, if `value` is in the specified range of `theArray`, otherwise `false`.

## See Also

### Examining an Array

func CFArrayBSearchValues(CFArray!, CFRange, UnsafeRawPointer!, CFComparatorFunction!, UnsafeMutableRawPointer!) -> CFIndex

Searches an array for a value using a binary search algorithm.

func CFArrayGetCount(CFArray!) -> CFIndex

Returns the number of values currently in an array.

func CFArrayGetCountOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Counts the number of times a given value occurs in an array.

func CFArrayGetFirstIndexOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Searches an array forward for a value.

func CFArrayGetLastIndexOfValue(CFArray!, CFRange, UnsafeRawPointer!) -> CFIndex

Searches an array backward for a value.

func CFArrayGetValues(CFArray!, CFRange, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from an array.

func CFArrayGetValueAtIndex(CFArray!, CFIndex) -> UnsafeRawPointer!

Retrieves a value at a given index.

