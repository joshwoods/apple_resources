

- Core Foundation
-  CFArrayGetCount(\_:) 

Function

# CFArrayGetCount(\_:)

Returns the number of values currently in an array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayGetCount(_ theArray: CFArray!) -> CFIndex
```

## Parameters 

`theArray`  

The array to examine.

## Return Value

The number of values in `theArray`.

## See Also

### Examining an Array

func CFArrayBSearchValues(CFArray!, CFRange, UnsafeRawPointer!, CFComparatorFunction!, UnsafeMutableRawPointer!) -> CFIndex

Searches an array for a value using a binary search algorithm.

func CFArrayContainsValue(CFArray!, CFRange, UnsafeRawPointer!) -> Bool

Reports whether or not a value is in an array.

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

