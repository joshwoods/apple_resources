

- os
- OSAllocatedUnfairLock
-  withLockUnchecked(flags:\_:) 

Instance Method

# withLockUnchecked(flags:\_:)

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func withLockUnchecked(
    flags: OSAllocatedUnfairLockFlags,
    _ body: (inout State) throws -> R
) rethrows -> R
```

