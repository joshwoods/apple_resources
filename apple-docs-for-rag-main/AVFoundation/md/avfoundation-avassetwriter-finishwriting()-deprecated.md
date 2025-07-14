

- AVFoundation
- AVAssetWriter
-  finishWriting() Deprecated

Instance Method

# finishWriting()

Completes the writing of the output file.

tvOS 9.0–9.0Deprecated

``` source
func finishWriting() -> Bool
```

Deprecated

Use finishWriting(completionHandler:) instead.

## Return Value

true if writing can be finished, otherwise false.

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

func cancelWriting()

Cancels the creation of the output file.

