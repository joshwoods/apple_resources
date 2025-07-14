

- AVFoundation
- AVAssetTrack
-  makeSampleCursor(presentationTimeStamp:) 

Instance Method

# makeSampleCursor(presentationTimeStamp:)

Creates a sample cursor and positions it at or near the specified presentation timestamp.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func makeSampleCursor(presentationTimeStamp: CMTime) -> AVSampleCursor?
```

## Parameters 

`presentationTimeStamp`  

The initial presentation timestamp of the sample cursor.

## Return Value

An instance of AVSampleCursor.

## Discussion

If the track’s asset property value for providesPreciseDurationAndTiming is true, the sample cursor is accurately positioned at the track’slast media sample with a presentation timestamp less than or equal to the desired timestamp, or, if there are no such samples, the first sample in presentation order.

If the track’s asset property value for providesPreciseDurationAndTiming is false, and it’s prohibitively expensive to locate the precise sample at the desired timestamp, the sample cursor may be approximately positioned.

## See Also

### Creating Sample Cursors

func makeSampleCursorAtFirstSampleInDecodeOrder() -> AVSampleCursor?

Creates a sample cursor and positions it at the track’s first media sample in decode order.

func makeSampleCursorAtLastSampleInDecodeOrder() -> AVSampleCursor?

Creates a sample cursor and positions it at the track’s last media sample in decode order.

