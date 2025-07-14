

- Core Foundation
-  CFBinaryHeapCallBacks 

Structure

# CFBinaryHeapCallBacks

Structure containing the callbacks for values for a `CFBinaryHeap` object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFBinaryHeapCallBacks
```

## Topics

### Initializers

init()

init(version: CFIndex, retain: ((CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?)!, release: ((CFAllocator?, UnsafeRawPointer?) -> Void)!, copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!, compare: ((UnsafeRawPointer?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> CFComparisonResult)!)

### Instance Properties

var compare: ((UnsafeRawPointer?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> CFComparisonResult)!

The callback used to compare values in the binary heap in some operations. This field cannot be `NULL`.

var copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!

Callback function used to get a description of a value in a binary heap.

var release: ((CFAllocator?, UnsafeRawPointer?) -> Void)!

Callback function used to release a value before it is removed from a binary heap.

var retain: ((CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?)!

Callback function used to retain a value being added to a binary heap.

var version: CFIndex

The version number of the structure type being passed in as a parameter to the `CFBinaryHeap` creation functions. This structure is version `0`.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct CFBinaryHeapCompareContext

Not used.

