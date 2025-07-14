

- Foundation
- Progress
-  cancel() 

Instance Method

# cancel()

Cancels progress tracking.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancel()
```

## Discussion

This method invokes the block for cancellationHandler, if there is one, and ensures that any subsequent reads of the isCancelled property return true.

If the receiver has suboperations, the system cancels their progress as well.

## See Also

### Controlling Progress

func pause()

Pauses progress tracking.

func resume()

Resumes progress tracking.

var resumingHandler: (() -> Void)?

The block to invoke when progress resumes.

