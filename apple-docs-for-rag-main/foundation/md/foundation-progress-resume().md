

- Foundation
- Progress
-  resume() 

Instance Method

# resume()

Resumes progress tracking.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func resume()
```

## Discussion

This method invokes the block for resumingHandler, if there is one, and ensures that any subsequent reads of the isPaused property return false.

If the receiver has suboperations, the system resumes their progress as well.

## See Also

### Controlling Progress

func cancel()

Cancels progress tracking.

func pause()

Pauses progress tracking.

var resumingHandler: (() -> Void)?

The block to invoke when progress resumes.

