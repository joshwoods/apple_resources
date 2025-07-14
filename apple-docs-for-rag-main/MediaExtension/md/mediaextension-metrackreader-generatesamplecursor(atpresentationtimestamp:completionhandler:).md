

- MediaExtension
- METrackReader
-  generateSampleCursor(atPresentationTimeStamp:completionHandler:) 

Instance Method

# generateSampleCursor(atPresentationTimeStamp:completionHandler:)

Provides a new sample cursor that points to the sample at or near the specified presentation timestamp.

macOS 14.0+

``` source
func generateSampleCursor(
    atPresentationTimeStamp presentationTimeStamp: CMTime,
    completionHandler: @escaping ((any MESampleCursor)?, (any Error)?) -> Void
)
```

``` source
func sampleCursor(atPresentationTimeStamp presentationTimeStamp: CMTime) async throws -> any MESampleCursor
```

**Required**

## Parameters 

`presentationTimeStamp`  

The presentation time stamp.

`completionHandler`  

The completion block to execute when the generate operation finishes.

## Discussion

The new sample cursor points to the last sample with a presentation time stamp (PTS) less than or equal to `presentationTimeStamp`, or if there are no such samples, the first sample in PTS order.

## See Also

### Getting track information

func loadTrackInfo(completionHandler: (METrackInfo?, (any Error)?) -> Void)

Loads the track info object with the properties of the media asset track.

**Required**

func generateSampleCursorAtFirstSampleInDecodeOrder(completionHandler: ((any MESampleCursor)?, (any Error)?) -> Void)

Provides a new sample cursor that points to the first sample in decode order.

**Required**

func generateSampleCursorAtLastSampleInDecodeOrder(completionHandler: ((any MESampleCursor)?, (any Error)?) -> Void)

Provides a new sample cursor that points to the last sample in decode order.

**Required**

func loadUneditedDuration(completionHandler: (CMTime, (any Error)?) -> Void)

Returns the duration of the track, disregarding edits.

func loadTotalSampleDataLength(completionHandler: (Int64, (any Error)?) -> Void)

Loads the total size in bytes of all the samples in the track.

func loadEstimatedDataRate(completionHandler: (Float32, (any Error)?) -> Void)

Loads the approximate data rate of the track in bytes per second.

func loadMetadata(completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads the array of metadata items from the media asset track.

