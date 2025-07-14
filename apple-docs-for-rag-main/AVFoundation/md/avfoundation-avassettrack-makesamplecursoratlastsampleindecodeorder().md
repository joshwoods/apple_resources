

- AVFoundation
- AVAssetTrack
-  makeSampleCursorAtLastSampleInDecodeOrder() 

Instance Method

# makeSampleCursorAtLastSampleInDecodeOrder()

Creates a sample cursor and positions it at the track’s last media sample in decode order.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func makeSampleCursorAtLastSampleInDecodeOrder() -> AVSampleCursor?
```

## Return Value

An instance of AVSampleCursor.

## See Also

### Creating Sample Cursors

func makeSampleCursor(presentationTimeStamp: CMTime) -> AVSampleCursor?

Creates a sample cursor and positions it at or near the specified presentation timestamp.

func makeSampleCursorAtFirstSampleInDecodeOrder() -> AVSampleCursor?

Creates a sample cursor and positions it at the track’s first media sample in decode order.

