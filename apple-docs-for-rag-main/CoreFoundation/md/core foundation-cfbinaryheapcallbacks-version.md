

- Core Foundation
- CFBinaryHeapCallBacks
-  version 

Instance Property

# version

The version number of the structure type being passed in as a parameter to the `CFBinaryHeap` creation functions. This structure is version `0`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var version: CFIndex
```

## See Also

### Callbacks

typealias CFBinaryHeapApplierFunction

Callback function used to apply a function to all members of a binary heap.

var compare: ((UnsafeRawPointer?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> CFComparisonResult)!

The callback used to compare values in the binary heap in some operations. This field cannot be `NULL`.

var copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!

Callback function used to get a description of a value in a binary heap.

var release: ((CFAllocator?, UnsafeRawPointer?) -> Void)!

Callback function used to release a value before it is removed from a binary heap.

var retain: ((CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?)!

Callback function used to retain a value being added to a binary heap.

