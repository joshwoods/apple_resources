

- Foundation
- Progress
-  completedUnitCount 

Instance Property

# completedUnitCount

The number of completed units of work for the current job.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var completedUnitCount: Int64 { get set }
```

## Discussion

For an Progress with a kind of file, the unit of this property is bytes, and the fileTotalCountKey and fileCompletedCountKey keys in the `userInfo` dictionary report the overall count of files.

For any other kind of Progress, the unit of measurement doesn’t matter as long as it’s consistent. You can report the values to the user in the localizedDescription and localizedAdditionalDescription.

## See Also

### Related Documentation

var fractionCompleted: Double

The fraction of the overall work that the progress object completes, including work from its suboperations.

### Reporting Progress

var totalUnitCount: Int64

The total number of tracked units of work for the current progress.

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

var pausingHandler: (() -> Void)?

The block to invoke when pausing progress.

