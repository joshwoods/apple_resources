

- Core Foundation
-  CFArrayCreateMutableCopy(\_:\_:\_:) 

Function

# CFArrayCreateMutableCopy(\_:\_:\_:)

Creates a new mutable array with the values from another array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayCreateMutableCopy(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ theArray: CFArray!
) -> CFMutableArray!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new array and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of values that can be contained by the new array. The array starts with the same number of values as `theArray` and can grow to this number of values (and it can have less).

Pass `0` to specify that the maximum capacity is not limited. If non-`0`, `capacity` must be greater than or equal to the count of `theArray`.

`theArray`  

The array to copy. The pointer values from the array are copied into the new array. However, the values are also retained by the new array.

## Return Value

A new mutable array that contains the same values as `theArray`. The new array has the same count as the `theArray` and uses the same callbacks. Ownership follows the The Create Rule.

## See Also

### CFMutableArray Miscellaneous Functions

func CFArrayAppendArray(CFMutableArray!, CFArray!, CFRange)

Adds the values from one array to another array.

func CFArrayAppendValue(CFMutableArray!, UnsafeRawPointer!)

Adds a value to an array giving it the new largest index.

func CFArrayCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFArrayCallBacks>!) -> CFMutableArray!

Creates a new empty mutable array.

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

