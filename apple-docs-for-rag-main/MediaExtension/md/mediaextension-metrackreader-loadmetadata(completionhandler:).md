

- MediaExtension
- METrackReader
-  loadMetadata(completionHandler:) 

Instance Method

# loadMetadata(completionHandler:)

Loads the array of metadata items from the media asset track.

macOS 14.0+

``` source
optional func loadMetadata(completionHandler: @escaping ([AVMetadataItem]?, (any Error)?) -> Void)
```

``` source
var metadata: [AVMetadataItem] { get async throws }
```

## Parameters 

`completionHandler`  

The completion block to execute when the load operation finishes.

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

func loadUneditedDuration(completionHandler: (CMTime, (any Error)?) -> Void)

Returns the duration of the track, disregarding edits.

func loadTotalSampleDataLength(completionHandler: (Int64, (any Error)?) -> Void)

Loads the total size in bytes of all the samples in the track.

func loadEstimatedDataRate(completionHandler: (Float32, (any Error)?) -> Void)

Loads the approximate data rate of the track in bytes per second.

