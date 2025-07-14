

- Foundation
- Progress
-  isPausable 

Instance Property

# isPausable

A Boolean value that indicates whether the receiver is tracking work that you can pause.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isPausable: Bool { get set }
```

## Discussion

By default, Progress objects aren’t pausable.

You typically use this property to communicate whether controls for pausing appear in a progress-reporting user interface. Progress itself doesn’t do anything with this property other than help pass the value from progress reporters to progress observers.

If an `NSProgress` is pausable, implement the ability to pause either by setting a block for the pausingHandler property, or by polling the isPaused property periodically while performing the relevant work.

It’s valid for the value of this property to change during the lifetime of an `NSProgress` object. By default, `NSProgress` is KVO-compliant for this property. It sends notifications on the same thread that updates the property.

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

var isPaused: Bool

A Boolean value that indicates whether the receiver is tracking paused work.

var pausingHandler: (() -> Void)?

The block to invoke when pausing progress.

