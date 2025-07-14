

- MediaExtension
- MESampleCursor
-  sampleLocation() 

Instance Method

# sampleLocation()

Returns the location and byte source of the sample indicated by the cursor.

macOS 14.0+

``` source
optional func sampleLocation() throws -> MESampleLocation
```

## Return Value

A sample location.

## Discussion

Sample data needs to be contiguous. If the sample data isn’t contiguous or the cursor doesn’t support this method, it fails with the error MEError.Code.locationNotAvailable. In this case, use loadSampleBufferContainingSamples(to:completionHandler:) to load the data.

If it’s not possible to implement this method, implement estimatedSampleLocation() to get an estimated sample location, and refineSampleLocation(_:refinementData:refinementDataLength:refinedLocation:) to analyze this data and provide precise location and size info.

## See Also

### Sending samples to a pipeline

func chunkDetails() throws -> MESampleCursorChunk

Returns information about the chunk that holds the sample indicated by the cursor.

func loadSampleBufferContainingSamples(to: (any MESampleCursor)?, completionHandler: (CMSampleBuffer?, (any Error)?) -> Void)

Builds a sample buffer that contains the samples at the cursor that you specify.

