

- Core Foundation
-  CFArrayInsertValueAtIndex(\_:\_:\_:) 

Function

# CFArrayInsertValueAtIndex(\_:\_:\_:)

Inserts a value into an array at a given index.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayInsertValueAtIndex(
    _ theArray: CFMutableArray!,
    _ idx: CFIndex,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theArray`  

The array into which `value` is inserted. If `theArray` is a fixed-capacity array and it is full before this operation, the behavior is undefined.

`idx`  

The index at which to insert `value`. The index must be in the range `0` to `N` inclusive, where `N` is the count of `theArray` before the operation. If the index is the same as the count of `theArray`, this function has the same effect as CFArrayAppendValue(_:_:).

`value`  

The value to insert into `theArray`. The value is retained by `theArray` using the retain callback provided when `theArray` was created. If `value` is not of the type expected by the retain callback, the behavior is undefined.

## Discussion

The `value` parameter is assigned to the index `idx`, and all values in `theArray` with equal and larger indices have their indices increased by one.

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

