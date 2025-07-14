

- Core Foundation
-  CFArrayRemoveAllValues(\_:) 

Function

# CFArrayRemoveAllValues(\_:)

Removes all the values from an array, making it empty.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayRemoveAllValues(_ theArray: CFMutableArray!)
```

## Parameters 

`theArray`  

The array from which all of the values are removed.

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

func CFArrayRemoveValueAtIndex(CFMutableArray!, CFIndex)

Removes the value at a given index from an array.

func CFArrayReplaceValues(CFMutableArray!, CFRange, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, CFIndex)

Replaces a range of values in an array.

func CFArraySetValueAtIndex(CFMutableArray!, CFIndex, UnsafeRawPointer!)

Changes the value at a given index in an array.

func CFArraySortValues(CFMutableArray!, CFRange, CFComparatorFunction!, UnsafeMutableRawPointer!)

Sorts the values in an array using a given comparison function.

