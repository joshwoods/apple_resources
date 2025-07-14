

- Foundation
- NSPointerFunctions
-  acquireFunction 

Instance Property

# acquireFunction

The function used to acquire memory.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var acquireFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?, ObjCBool) -> UnsafeMutableRawPointer)? { get set }
```

## Discussion

This specifies the function to use for copy-in operations.

## See Also

### Memory Configuration

var relinquishFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> Void)?

The function used to relinquish memory.

var usesStrongWriteBarrier: Bool

Specifies whether, in a garbage collected environment, pointers should be assigned using a strong write barrier.

Deprecated

var usesWeakReadAndWriteBarriers: Bool

Specifies whether, in a garbage collected environment, pointers should use weak read and write barriers.

Deprecated

