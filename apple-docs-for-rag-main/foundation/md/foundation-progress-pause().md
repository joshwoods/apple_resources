

- Foundation
- Progress
-  pause() 

Instance Method

# pause()

Pauses progress tracking.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func pause()
```

## Discussion

This method invokes the block for pausingHandler, if there is one, and ensures that any subsequent reads of the isPaused property return true.

If the receiver has suboperations, the system pauses their progress as well.

## See Also

### Controlling Progress

func cancel()

Cancels progress tracking.

func resume()

Resumes progress tracking.

var resumingHandler: (() -> Void)?

The block to invoke when progress resumes.

