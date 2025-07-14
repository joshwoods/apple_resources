

- MediaExtension
- MESampleCursor
-  chunkDetails() 

Instance Method

# chunkDetails()

Returns information about the chunk that holds the sample indicated by the cursor.

macOS 14.0+

``` source
optional func chunkDetails() throws -> MESampleCursorChunk
```

## Return Value

A sample cursor chunk.

## Discussion

If the sample resides in a contiguous chunk of the file among similar samples, this method returns information about that chunk.

Note

If a cursor implements this method, it also needs to implement sampleLocation() to get samples inside the chunk’s location.

It may not be practical to use this method with some media assets. In this case, or if the cursor doesn’t support this method, it returns MEError.Code.locationNotAvailable, which indicates to use loadSampleBufferContainingSamples(to:completionHandler:) to load the sample data instead.

## See Also

### Sending samples to a pipeline

func sampleLocation() throws -> MESampleLocation

Returns the location and byte source of the sample indicated by the cursor.

func loadSampleBufferContainingSamples(to: (any MESampleCursor)?, completionHandler: (CMSampleBuffer?, (any Error)?) -> Void)

Builds a sample buffer that contains the samples at the cursor that you specify.

