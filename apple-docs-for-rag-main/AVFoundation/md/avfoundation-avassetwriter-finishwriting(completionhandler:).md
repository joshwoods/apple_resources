

- AVFoundation
- AVAssetWriter
-  finishWriting(completionHandler:) 

Instance Method

# finishWriting(completionHandler:)

Marks all unfinished inputs as finished and completes the writing of the output file.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func finishWriting(completionHandler handler: @escaping () -> Void)
```

``` source
func finishWriting() async
```

## Parameters 

`handler`  

A completion handler the system invokes when it finishes writing. Determine the success or failure of the writing session by querying the asset writer’s status property value.

## Discussion

To ensure the asset writer finishes writing all samples, call this method only after all calls to append(_:) or append(_:withPresentationTime:) return.

## See Also

### Managing Writing Sessions

func startWriting() -> Bool

Tells the writer to start writing its output.

func startSession(atSourceTime: CMTime)

Starts an asset-writing session.

func endSession(atSourceTime: CMTime)

Finishes an asset-writing session.

func cancelWriting()

Cancels the creation of the output file.

func finishWriting() -> Bool

Completes the writing of the output file.

Deprecated

