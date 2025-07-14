

- AVFoundation
- AVAssetWriter
-  endSession(atSourceTime:) 

Instance Method

# endSession(atSourceTime:)

Finishes an asset-writing session.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func endSession(atSourceTime endTime: CMTime)
```

## Parameters 

`endTime`  

The ending asset time for the session, in the timeline of the source samples.

## Discussion

Call this method to complete a session that you started with startSession(atSourceTime:).

The end time defines the moment on the timeline of source samples at which the session ends. In the case of the QuickTime movie file format, each sample-writing session’s start and end time pair corresponds to a period of movie time into which a writer inserts samples. The writer adds samples with timestamps that are later than the session end time to the written file but they aren’t presented during playback. For example, if the first session has duration `D1 = endTime - startTime`, the writer inserts it into the written file at time `0` through `D1`; the second session would insert into the written file at time `D1` through `D1 + D2`, and so on. It’s legal to have a session with no samples; this causes the creation of an empty edit of the prescribed duration.

If you don’t explicitly call this method, the system invokes it automatically when you call finishWriting(completionHandler:). In that case, the session’s effective end time is the timestamp of the last sample you append.

Note

An asset writer doesn’t support multiple sample-writing sessions. It’s an error to call startSession(atSourceTime:) a second time after calling endSession(atSourceTime:).

## See Also

### Managing Writing Sessions

func startWriting() -> Bool

Tells the writer to start writing its output.

func startSession(atSourceTime: CMTime)

Starts an asset-writing session.

func finishWriting(completionHandler: () -> Void)

Marks all unfinished inputs as finished and completes the writing of the output file.

func cancelWriting()

Cancels the creation of the output file.

func finishWriting() -> Bool

Completes the writing of the output file.

Deprecated

