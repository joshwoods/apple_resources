

- Swift
- Clock
-  continuous 

Type Property

# continuous

A clock that measures time that always increments but does not stop incrementing while the system is asleep.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var continuous: ContinuousClock { get }
```

Available when `Self` is `ContinuousClock`.

## Discussion

```
  try await Task.sleep(until: .now + .seconds(3), clock: .continuous)
```

