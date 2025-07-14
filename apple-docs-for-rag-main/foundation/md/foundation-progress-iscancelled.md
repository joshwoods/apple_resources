

- Foundation
- Progress
-  isCancelled 

Instance Property

# isCancelled

A Boolean value that Indicates whether the receiver is tracking canceled work.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isCancelled: Bool { get }
```

## Discussion

By default, Progress is KVO-compliant for this property. It sends notifications on the same thread that updates the property.

If the receiver has a canceled containing progress object, the receiver reports a canceled status.

## See Also

### Related Documentation

func cancel()

Cancels progress tracking.

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

var cancellationHandler: (() -> Void)?

The block to invoke when canceling progress.

var isPausable: Bool

A Boolean value that indicates whether the receiver is tracking work that you can pause.

var isPaused: Bool

A Boolean value that indicates whether the receiver is tracking paused work.

var pausingHandler: (() -> Void)?

The block to invoke when pausing progress.

