

- Core Foundation
-  CFArrayAppendArray(\_:\_:\_:) 

Function

# CFArrayAppendArray(\_:\_:\_:)

Adds the values from one array to another array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayAppendArray(
    _ theArray: CFMutableArray!,
    _ otherArray: CFArray!,
    _ otherRange: CFRange
)
```

## Parameters 

`theArray`  

The array to which values from `otherArray` are added. If `theArray` is a limited-capacity array, adding `otherRange.length` values from `otherArray` must not cause the capacity limit of `theArray` to be exceeded.

`otherArray`  

An array providing the values to be added to `theArray`.

`otherRange`  

The range within `otherArray` from which to add the values to `theArray`. The range must not exceed the index space of `otherArray`.

## Discussion

The new values are retained by `theArray` using the retain callback provided when `theArray` was created. If the values are not of the type expected by the retain callback, the behavior is undefined. The values are assigned to the indices one larger than the previous largest index in `theArray`, and beyond, and the count of `theArray` is increased by `otherRange.length`. The values are assigned new indices in `theArray` from smallest to largest index in the order in which they appear in `otherArray`.

## See Also

### CFMutableArray Miscellaneous Functions

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

func CFArraySetValueAtIndex(CFMutableArray!, CFIndex, UnsafeRawPointer!)

Changes the value at a given index in an array.

func CFArraySortValues(CFMutableArray!, CFRange, CFComparatorFunction!, UnsafeMutableRawPointer!)

Sorts the values in an array using a given comparison function.

