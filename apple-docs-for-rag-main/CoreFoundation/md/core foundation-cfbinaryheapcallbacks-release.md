

- Core Foundation
- CFBinaryHeapCallBacks
-  release 

Instance Property

# release

Callback function used to release a value before it is removed from a binary heap.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var release: ((CFAllocator?, UnsafeRawPointer?) -> Void)!
```

## Parameters 

`allocator`  

The binary heap’s allocator.

`ptr`  

The value to release.

## Discussion

The callback used to remove a retain previously added for the binary heap from values as they are removed from the binary heap. If this field is `NULL`, the binary heap does nothing to release a value being removed.

## See Also

### Callbacks

typealias CFBinaryHeapApplierFunction

Callback function used to apply a function to all members of a binary heap.

var compare: ((UnsafeRawPointer?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> CFComparisonResult)!

The callback used to compare values in the binary heap in some operations. This field cannot be `NULL`.

var copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!

Callback function used to get a description of a value in a binary heap.

var retain: ((CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?)!

Callback function used to retain a value being added to a binary heap.

var version: CFIndex

The version number of the structure type being passed in as a parameter to the `CFBinaryHeap` creation functions. This structure is version `0`.

