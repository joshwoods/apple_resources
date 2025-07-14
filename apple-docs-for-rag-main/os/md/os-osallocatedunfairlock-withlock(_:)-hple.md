

- os
- OSAllocatedUnfairLock
-  withLock(\_:) 

Instance Method

# withLock(\_:)

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func withLock(_ body: () throws -> R) rethrows -> R where R : Sendable
```

Available when `State` is `()`.

