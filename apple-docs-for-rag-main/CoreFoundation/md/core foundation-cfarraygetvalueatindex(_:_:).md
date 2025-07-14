

- Core Foundation
-  CFArrayGetValueAtIndex(\_:\_:) 

Function

# CFArrayGetValueAtIndex(\_:\_:)

Retrieves a value at a given index.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayGetValueAtIndex(
    _ theArray: CFArray!,
    _ idx: CFIndex
) -> UnsafeRawPointer!
```

## Parameters 

`theArray`  

The array to examine.

`idx`  

The index of the value to retrieve. If the index is outside the index space of `theArray` (`0` to `N-1` inclusive (where `N` is the count of `theArray`), the behavior is undefined.

## Return Value

The value at the `idx` index in `theArray`. If the return value is a Core Foundation Object, ownership follows The Get Rule.

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

func CFArrayGetValues(CFArray!, CFRange, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from an array.

