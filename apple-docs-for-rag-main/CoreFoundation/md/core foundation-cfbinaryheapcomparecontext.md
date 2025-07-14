

- Core Foundation
-  CFBinaryHeapCompareContext 

Structure

# CFBinaryHeapCompareContext

Not used.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFBinaryHeapCompareContext
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: ((UnsafeRawPointer?) -> UnsafeRawPointer?)!, release: ((UnsafeRawPointer?) -> Void)!, copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!)

### Instance Properties

var copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!

var info: UnsafeMutableRawPointer!

var release: ((UnsafeRawPointer?) -> Void)!

var retain: ((UnsafeRawPointer?) -> UnsafeRawPointer?)!

var version: CFIndex

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct CFBinaryHeapCallBacks

Structure containing the callbacks for values for a `CFBinaryHeap` object.

