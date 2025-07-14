

- Foundation
- OperationQueue
-  progress 

Instance Property

# progress

An object that represents the total progress of the operations executing in the queue.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var progress: Progress { get }
```

## Discussion

By default, OperationQueue doesn’t report progress until totalUnitCount is set. When totalUnitCount is set, the queue begins reporting progress. Each operation in the queue contributes one unit of completion to the overall progress of the queue for operations that are finished by the end of main(). Operations that override start() and don’t invoke super don’t contribute to the queue’s progress.

Warning

Be careful to avoid race conditions and backward progress when updating totalUnitCount. Consider a queue with a progress that has a completedUnitCount equal to `5` and a totalUnitCount equal to `10`, representing 50% completion. If you add 90 more operations to the queue, the totalUnitCount is now `100`, and the progress completion reports 5%. If the progress object is connected to a progress bar, the bar would visibly jump backward from 50% to 5%, which may not be desirable.

To update totalUnitCount in a thread-safe manner, use the addBarrierBlock(_:) method. This method ensures that the operation queue completes the operations in the queue, preventing an inadvertent backward jump in progress.

