

- TipKit
- Tip
-  shouldDisplayUpdates 

Instance Property

# shouldDisplayUpdates

An asynchronous sequence for monitoring a tip’s display eligibility.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var shouldDisplayUpdates: AsyncMapSequence, Bool> { get }
```

## See Also

### Monitoring tip status

var status: Self.Status

The current status of a tip based on its rules and the configured displayFrequency(_:).

var statusUpdates: AsyncStream&lt;Self.Status>

An asynchronous sequence for monitoring a tip’s status changes.

var shouldDisplay: Bool

A Boolean value that determines whether to display a tip.

typealias Status

A type that describes the current display eligibility status for a tip.

typealias InvalidationReason

A type that describes why the system permanently invalidated a tip.

