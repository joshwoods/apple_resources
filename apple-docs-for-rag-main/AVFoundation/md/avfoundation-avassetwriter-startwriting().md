

- AVFoundation
- AVAssetWriter
-  startWriting() 

Instance Method

# startWriting()

Tells the writer to start writing its output.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func startWriting() -> Bool
```

## Return Value

true if writing starts successfully; otherwise false.

## Discussion

You must call this method after you configure the writer and add its inputs to prepare the object to write data. After you call this method, your app can start writing sessions by calling startSession(atSourceTime:) and can write media samples using the methods that the asset writer’s inputs provide.

If writing fails to start, this method returns false. In this case, check the values of the status and error properties to determine the reason for the failure.

## See Also

### Managing Writing Sessions

func startSession(atSourceTime: CMTime)

Starts an asset-writing session.

func endSession(atSourceTime: CMTime)

Finishes an asset-writing session.

func finishWriting(completionHandler: () -> Void)

Marks all unfinished inputs as finished and completes the writing of the output file.

func cancelWriting()

Cancels the creation of the output file.

func finishWriting() -> Bool

Completes the writing of the output file.

Deprecated

