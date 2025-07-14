

- Foundation
- Progress
-  isCancellable 

Instance Property

# isCancellable

A Boolean value that indicates whether the receiver is tracking work that you can cancel.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isCancellable: Bool { get set }
```

## Discussion

By default, Progress objects are cancelable.

You typically use this property to communicate whether controls for canceling appear in a progress-reporting user interface. Progress itself doesn’t do anything with this property other than help pass the value from progress reporters to progress observers.

If an Progress is cancelable, implement the ability to cancel progress either by setting a block for the cancellationHandler property, or by polling the isCancelled property periodically while performing the relevant work.

It’s valid for the value of this property to change during the lifetime of an Progress object. By default, Progress is KVO-compliant for this property. It sends notifications on the same thread that updates the property.

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

var isCancelled: Bool

A Boolean value that Indicates whether the receiver is tracking canceled work.

var cancellationHandler: (() -> Void)?

The block to invoke when canceling progress.

var isPausable: Bool

A Boolean value that indicates whether the receiver is tracking work that you can pause.

var isPaused: Bool

A Boolean value that indicates whether the receiver is tracking paused work.

var pausingHandler: (() -> Void)?

The block to invoke when pausing progress.

