

- Foundation
- Progress
-  pausingHandler 

Instance Property

# pausingHandler

The block to invoke when pausing progress.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var pausingHandler: (() -> Void)? { get set }
```

## Discussion

If the receiver is a suboperation of another progress object, the system invokes the pausingHandler block when pausing the containing progress object.

### Special Considerations

You’re responsible for pausing any work for the progress object.

You can invoke the pausing handler on any queue. If you must do work on a specific queue, dispatch to that queue from within the pausing handler block.

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

var isPaused: Bool

A Boolean value that indicates whether the receiver is tracking paused work.

