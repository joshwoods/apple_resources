

- Swift
- ContinuousClock
-  sleep(for:tolerance:) 

Instance Method

# sleep(for:tolerance:)

Suspends for the given duration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func sleep(
    for duration: Self.Instant.Duration,
    tolerance: Self.Instant.Duration? = nil
) async throws
```

## Discussion

Prefer to use the `sleep(until:tolerance:)` method on `Clock` if you have access to an absolute instant.

