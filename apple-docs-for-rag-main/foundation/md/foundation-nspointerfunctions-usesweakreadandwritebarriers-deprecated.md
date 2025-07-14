

- Foundation
- NSPointerFunctions
-  usesWeakReadAndWriteBarriers Deprecated

Instance Property

# usesWeakReadAndWriteBarriers

Specifies whether, in a garbage collected environment, pointers should use weak read and write barriers.

iOS 2.0–10.0DeprecatediPadOS 2.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
var usesWeakReadAndWriteBarriers: Bool { get set }
```

Deprecated

Garbage collection no longer supported

## Discussion

If you use garbage collection, read and write barrier functions must be used when pointers are from memory scanned by the collector.

## See Also

### Memory Configuration

var acquireFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?, ObjCBool) -> UnsafeMutableRawPointer)?

The function used to acquire memory.

var relinquishFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> Void)?

The function used to relinquish memory.

var usesStrongWriteBarrier: Bool

Specifies whether, in a garbage collected environment, pointers should be assigned using a strong write barrier.

Deprecated

