

- Swift
- SuspendingClock
-  measure(isolation:\_:) 

Instance Method

# measure(isolation:\_:)

Measure the elapsed time to execute an asynchronous closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func measure(
    isolation: isolated (any Actor)? = #isolation,
    _ work: () async throws -> Void
) async rethrows -> Self.Instant.Duration
```

## Discussion

```
  let clock = ContinuousClock()
  let elapsed = await clock.measure {
     await someWork()
  }
```

