

- Swift
- Clock
-  suspending 

Type Property

# suspending

A clock that measures time that always increments but stops incrementing while the system is asleep.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var suspending: SuspendingClock { get }
```

Available when `Self` is `SuspendingClock`.

## Discussion

```
  try await Task.sleep(until: .now + .seconds(3), clock: .suspending)
```

