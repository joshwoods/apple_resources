

- AVFoundation
- AVAssetWriter
-  startSession(atSourceTime:) 

Instance Method

# startSession(atSourceTime:)

Starts an asset-writing session.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func startSession(atSourceTime startTime: CMTime)
```

## Parameters 

`startTime`  

The starting asset time for the sample-writing session, in the timeline of the source samples.

## Discussion

You must call this method after you call startWriting(), but before you append sample data to asset writer inputs.

Each writing session has a start time that, where allowed by the file format you’re writing, defines the mapping from the timeline of source samples to the timeline of the written file. In the case of the QuickTime movie file format, the first session begins at movie time `0`, so a sample you append with timestamp `T` plays at movie time (`T-startTime`). The writer adds samples with timestamps earlier than the start time to the output file, but they don’t display during playback. If the earliest sample for an input has a timestamp later than the start time, the system inserts an empty edit to preserve synchronization between tracks of the output asset.

To end a session, call endSession(atSourceTime:)or finishWriting(completionHandler:)

Note

An asset writer doesn’t support multiple sample-writing sessions. It’s an error to call startSession(atSourceTime:) a second time after calling endSession(atSourceTime:).

## See Also

### Managing Writing Sessions

func startWriting() -> Bool

Tells the writer to start writing its output.

func endSession(atSourceTime: CMTime)

Finishes an asset-writing session.

func finishWriting(completionHandler: () -> Void)

Marks all unfinished inputs as finished and completes the writing of the output file.

func cancelWriting()

Cancels the creation of the output file.

func finishWriting() -> Bool

Completes the writing of the output file.

Deprecated

