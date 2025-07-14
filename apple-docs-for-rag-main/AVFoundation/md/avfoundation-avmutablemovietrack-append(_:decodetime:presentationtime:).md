

- AVFoundation
- AVMutableMovieTrack
-  append(\_:decodeTime:presentationTime:) 

Instance Method

# append(\_:decodeTime:presentationTime:)

Appends sample data to a media file and adds sample references for the added data to a track’s media sample tables.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 6.0+

``` source
func append(
    _ sampleBuffer: CMSampleBuffer,
    decodeTime outDecodeTime: UnsafeMutablePointer?,
    presentationTime outPresentationTime: UnsafeMutablePointer?
) throws
```

## Parameters 

`sampleBuffer`  

The sample buffer to be appended.

`outDecodeTime`  

A pointer to a CMTime structure to receive the decode time in the media of the first sample appended from the sample buffer. Pass `NULL` if the information is not needed.

`outPresentationTime`  

A pointer to a CMTime structure to receive the presentation time in the media of the first sample appended from the sample buffer. Pass `NULL` if the information is not needed.

## Discussion

If the sample buffer carries sample data, the sample data is written to the container specified by the track property mediaDataStorage if non-nil, or by the movie property defaultMediaDataStorage if non-nil, and sample references are appended to the track’s media. If both media data storage properties are `nil`, the method will fail and return `NO`.

If the sample buffer carries sample references only, sample data will not be written and sample references to the samples in their original container are appended to the track’s media as necessary.

Note

In a track’s media, the first sample’s decode timestamp must be zero. For an audio track, each sample buffer’s duration is used as the sample decode duration. For other track types, the difference between a sample’s decode timestamp and the following sample’s decode timestamp is used as the first sample’s decode duration, so as to preserve the relative timing.

To make the new samples appear in the track’s timeline, invoke insertMediaTimeRange(_:into:). Retrieve the mediaPresentationTimeRange property before and after appending a sequence of samples, using CMTimeRangeGetEnd(_:) on each to calculate the media time range for insertMediaTimeRange(_:into:).

It’s safe for multiple threads to call this method on different tracks at the same time.

## See Also

### Appending Sample Data

func insertMediaTimeRange(CMTimeRange, into: CMTimeRange) -> Bool

Inserts a reference to a media time range into a track.

