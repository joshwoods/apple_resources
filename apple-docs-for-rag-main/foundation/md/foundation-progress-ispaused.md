

- Foundation
- Progress
-  isPaused 

Instance Property

# isPaused

A Boolean value that indicates whether the receiver is tracking paused work.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isPaused: Bool { get }
```

## Discussion

By default, `NSProgress` is KVO-compliant for this property. It sends notifications on the same thread that updates the property.

If the receiver has a paused containing progress object, the receiver reports a paused status.

## See Also

### Reporting Progress

var totalUnitCount: Int64

The total number of tracked units of work for the current progress.

var completedUnitCount: Int64

The number of completed units of work for the current job.

var localizedDescription: String!

A localized description of tracked progress for the receiver.

var localizedAdditionalDescription: String!

A more specific localized description of tracked progress for the receiver.

var isCancellable: Bool

A Boolean value that indicates whether the receiver is tracking work that you can cancel.

var isCancelled: Bool

A Boolean value that Indicates whether the receiver is tracking canceled work.

var cancellationHandler: (() -> Void)?

The block to invoke when canceling progress.

var isPausable: Bool

A Boolean value that indicates whether the receiver is tracking work that you can pause.

var pausingHandler: (() -> Void)?

The block to invoke when pausing progress.

