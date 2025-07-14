

- Core Foundation
-  CFArrayCreateMutable(\_:\_:\_:) 

Function

# CFArrayCreateMutable(\_:\_:\_:)

Creates a new empty mutable array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayCreateMutable(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ callBacks: UnsafePointer!
) -> CFMutableArray!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new array and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of values that can be contained by the new array. The array starts empty and can grow to this number of values (and it can have less).

Pass `0` to specify that the maximum capacity is not limited. The value must not be negative.

`callBacks`  

A pointer to a CFArrayCallBacks structure initialized with the callbacks for the array to use on each value in the array. A copy of the contents of the callbacks structure is made, so that a pointer to a structure on the stack can be passed in or can be reused for multiple array creations.

If the array contains CFType objects only, then pass kCFTypeArrayCallBacks to use the default callback functions.

This parameter may be `NULL`, which is treated as if a valid structure of version `0` with all fields `NULL` had been passed in.

If any of the fields are not valid pointers to functions of the correct type, or this parameter is not a valid pointer to a `CFArrayCallBacks` structure, the behavior is undefined. If any value put into the array is not one understood by one of the callback functions, the behavior when that callback function is used is undefined.

## Return Value

A new mutable array, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### CFMutableArray Miscellaneous Functions

func CFArrayAppendArray(CFMutableArray!, CFArray!, CFRange)

Adds the values from one array to another array.

func CFArrayAppendValue(CFMutableArray!, UnsafeRawPointer!)

Adds a value to an array giving it the new largest index.

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

