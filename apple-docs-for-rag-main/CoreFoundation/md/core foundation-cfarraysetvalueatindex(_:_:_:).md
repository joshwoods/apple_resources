

- Core Foundation
-  CFArraySetValueAtIndex(\_:\_:\_:) 

Function

# CFArraySetValueAtIndex(\_:\_:\_:)

Changes the value at a given index in an array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArraySetValueAtIndex(
    _ theArray: CFMutableArray!,
    _ idx: CFIndex,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theArray`  

The array in which the value is to be changed.

`idx`  

The index at which to set the new value. The value must not lie outside the index space of `theArray` (`0` to `N-1` inclusive, where `N` is the count of the array before the operation).

`value`  

The value to set in `theArray`. The value is retained by `theArray` using the retain callback provided when `theArray` was created and the previous value at `idx` is released. If the value is not of the type expected by the retain callback, the behavior is undefined. The indices of other values are not affected.

## See Also

### CFMutableArray Miscellaneous Functions

func CFArrayAppendArray(CFMutableArray!, CFArray!, CFRange)

Adds the values from one array to another array.

func CFArrayAppendValue(CFMutableArray!, UnsafeRawPointer!)

Adds a value to an array giving it the new largest index.

func CFArrayCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFArrayCallBacks>!) -> CFMutableArray!

Creates a new empty mutable array.

func CFArrayCreateMutableCopy(CFAllocator!, CFIndex, CFArray!) -> CFMutableArray!

Creates a new mutable array with the values from another array.

func CFArrayExchangeValuesAtIndices(CFMutableArray!, CFIndex, CFIndex)

Exchanges the values at two indices of an array.

func CFArrayInsertValueAtIndex(CFMutableArray!, CFIndex, UnsafeRawPointer!)

Inserts a value into an array at a given index.

func CFArrayRemoveAllValues(CFMutableArray!)

Removes all the values from an array, making it empty.

func CFArrayRemoveValueAtIndex(CFMutableArray!, CFIndex)

Removes the value at a given index from an array.

func CFArrayReplaceValues(CFMutableArray!, CFRange, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, CFIndex)

Replaces a range of values in an array.

func CFArraySortValues(CFMutableArray!, CFRange, CFComparatorFunction!, UnsafeMutableRawPointer!)

Sorts the values in an array using a given comparison function.

