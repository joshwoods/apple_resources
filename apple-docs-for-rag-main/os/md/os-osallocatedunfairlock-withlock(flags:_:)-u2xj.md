

- os
- OSAllocatedUnfairLock
-  withLock(flags:\_:) 

Instance Method

# withLock(flags:\_:)

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func withLock(
    flags: OSAllocatedUnfairLockFlags,
    _ body: () throws -> R
) rethrows -> R where R : Sendable
```

Available when `State` is `()`.

