

- Core Foundation
-  CFArrayBSearchValues(\_:\_:\_:\_:\_:) 

Function

# CFArrayBSearchValues(\_:\_:\_:\_:\_:)

Searches an array for a value using a binary search algorithm.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayBSearchValues(
    _ theArray: CFArray!,
    _ range: CFRange,
    _ value: UnsafeRawPointer!,
    _ comparator: CFComparatorFunction!,
    _ context: UnsafeMutableRawPointer!
) -> CFIndex
```

## Parameters 

`theArray`  

An array, sorted from least to greatest according to the `comparator` function.

`range`  

The range within `theArray` to search. The range must not exceed the bounds of `theArray`. The range may be empty (length `0`).

`value`  

The value for which to find a match in `theArray`. If `value`, or any other value in `theArray`, is not understood by the `comparator` callback, the behavior is undefined.

`comparator`  

The function with the comparator function type signature that is used in the binary search operation to compare values in `theArray` with the given value. If there are values in the range that the `comparator` function does not expect or cannot properly compare, the behavior is undefined.

`context`  

A pointer-sized program-defined value, which is passed as the third argument to the `comparator` function, but is otherwise unused by this function. If the context is not what is expected by the `comparator` function, the behavior is undefined.

## Return Value

The return value is one of the following:

## Discussion

- The index of a value that matched, if the target value matches one or more in the range.

- Greater than or equal to the end point of the range, if the value is greater than all the values in the range.

- The index of the value greater than the target value, if the value lies between two of (or less than all of) the values in the range.

## See Also

### Examining an Array

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

func CFArrayGetValues(CFArray!, CFRange, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from an array.

func CFArrayGetValueAtIndex(CFArray!, CFIndex) -> UnsafeRawPointer!

Retrieves a value at a given index.

