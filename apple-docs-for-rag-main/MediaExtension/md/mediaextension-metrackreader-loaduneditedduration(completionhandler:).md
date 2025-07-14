

- MediaExtension
- METrackReader
-  loadUneditedDuration(completionHandler:) 

Instance Method

# loadUneditedDuration(completionHandler:)

Returns the duration of the track, disregarding edits.

macOS 14.0+

``` source
optional func loadUneditedDuration(completionHandler: @escaping (CMTime, (any Error)?) -> Void)
```

``` source
var uneditedDuration: CMTime { get async throws }
```

## Parameters 

`completionHandler`  

The completion block to execute when the load operation finishes.

## Discussion

Media Toolbox uses this information to validate edit information and to check if the media is suitable for gapless playback.

## See Also

### Getting track information

func loadTrackInfo(completionHandler: (METrackInfo?, (any Error)?) -> Void)

Loads the track info object with the properties of the media asset track.

**Required**

func generateSampleCursor(atPresentationTimeStamp: CMTime, completionHandler: ((any MESampleCursor)?, (any Error)?) -> Void)

Provides a new sample cursor that points to the sample at or near the specified presentation timestamp.

**Required**

func generateSampleCursorAtFirstSampleInDecodeOrder(completionHandler: ((any MESampleCursor)?, (any Error)?) -> Void)

Provides a new sample cursor that points to the first sample in decode order.

**Required**

func generateSampleCursorAtLastSampleInDecodeOrder(completionHandler: ((any MESampleCursor)?, (any Error)?) -> Void)

Provides a new sample cursor that points to the last sample in decode order.

**Required**

func loadTotalSampleDataLength(completionHandler: (Int64, (any Error)?) -> Void)

Loads the total size in bytes of all the samples in the track.

func loadEstimatedDataRate(completionHandler: (Float32, (any Error)?) -> Void)

Loads the approximate data rate of the track in bytes per second.

func loadMetadata(completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads the array of metadata items from the media asset track.

