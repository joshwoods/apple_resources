

- AVFoundation
- AVAssetWriter
-  cancelWriting() 

Instance Method

# cancelWriting()

Cancels the creation of the output file.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func cancelWriting()
```

## Discussion

If the asset writer is in AVAssetWriter.Status.failed or AVAssetWriter.Status.completed state, calling this method has no effect. Otherwise, invoking it blocks the calling thread until the asset writer finishes canceling the writing session.

If the asset writer created an output file during the writing process, calling this method deletes the file.

## See Also

### Managing Writing Sessions

func startWriting() -> Bool

Tells the writer to start writing its output.

func startSession(atSourceTime: CMTime)

Starts an asset-writing session.

func endSession(atSourceTime: CMTime)

Finishes an asset-writing session.

func finishWriting(completionHandler: () -> Void)

Marks all unfinished inputs as finished and completes the writing of the output file.

func finishWriting() -> Bool

Completes the writing of the output file.

Deprecated

