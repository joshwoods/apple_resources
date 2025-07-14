

- MediaExtension
- METrackReader
-  loadEstimatedDataRate(completionHandler:) 

Instance Method

# loadEstimatedDataRate(completionHandler:)

Loads the approximate data rate of the track in bytes per second.

macOS 14.0+

``` source
optional func loadEstimatedDataRate(completionHandler: @escaping (Float32, (any Error)?) -> Void)
```

``` source
var estimatedDataRate: Float32 { get async throws }
```

## Parameters 

`completionHandler`  

The completion block to execute when the load operation finishes.

## Discussion

If this method fails, it sets `estimatedDataRate` to `0.0` and the error contains information about the failure.

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

func loadMetadata(completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads the array of metadata items from the media asset track.

