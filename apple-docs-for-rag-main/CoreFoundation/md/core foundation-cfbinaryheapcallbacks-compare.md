

- Core Foundation
- CFBinaryHeapCallBacks
-  compare 

Instance Property

# compare

The callback used to compare values in the binary heap in some operations. This field cannot be `NULL`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var compare: ((UnsafeRawPointer?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> CFComparisonResult)!
```

## Parameters 

`ptr1`  

First value to compare.

`ptr2`  

Second value to compare.

`info`  

Not used. Should always be `NULL`.

## Return Value

CFComparisonResult.compareLessThan if `ptr1` is less than `ptr2`, CFComparisonResult.compareEqualTo if `ptr1` and `ptr2` are equal, or CFComparisonResult.compareGreaterThan if `ptr1` is greater than `ptr2`.

## See Also

### Callbacks

typealias CFBinaryHeapApplierFunction

Callback function used to apply a function to all members of a binary heap.

var copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!

Callback function used to get a description of a value in a binary heap.

var release: ((CFAllocator?, UnsafeRawPointer?) -> Void)!

Callback function used to release a value before it is removed from a binary heap.

var retain: ((CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?)!

Callback function used to retain a value being added to a binary heap.

var version: CFIndex

The version number of the structure type being passed in as a parameter to the `CFBinaryHeap` creation functions. This structure is version `0`.

