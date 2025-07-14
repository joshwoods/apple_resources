

- Foundation
- NSPointerFunctions
-  relinquishFunction 

Instance Property

# relinquishFunction

The function used to relinquish memory.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var relinquishFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> Void)? { get set }
```

## Discussion

This specifies the function to use when an item is removed from a table or pointer array.

## See Also

### Memory Configuration

var acquireFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?, ObjCBool) -> UnsafeMutableRawPointer)?

The function used to acquire memory.

var usesStrongWriteBarrier: Bool

Specifies whether, in a garbage collected environment, pointers should be assigned using a strong write barrier.

Deprecated

var usesWeakReadAndWriteBarriers: Bool

Specifies whether, in a garbage collected environment, pointers should use weak read and write barriers.

Deprecated

