

- Foundation
- Progress
-  resumingHandler 

Instance Property

# resumingHandler

The block to invoke when progress resumes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var resumingHandler: (() -> Void)? { get set }
```

## Discussion

If the receiver is a suboperation of another progress object, the system invokes the resumingHandler block when pausing the containing progress object.

### Special Considerations

You’re responsible for resuming any work for the progress object.

You can invoke the resuming handler on any queue. If you must do work on a specific queue, dispatch to that queue from within the resuming handler block.

## See Also

### Controlling Progress

func cancel()

Cancels progress tracking.

func pause()

Pauses progress tracking.

func resume()

Resumes progress tracking.

