

- MediaExtension
- MESampleCursor
-  loadSampleBufferContainingSamples(to:completionHandler:) 

Instance Method

# loadSampleBufferContainingSamples(to:completionHandler:)

Builds a sample buffer that contains the samples at the cursor that you specify.

macOS 14.0+

``` source
optional func loadSampleBufferContainingSamples(
    to endSampleCursor: (any MESampleCursor)?,
    completionHandler: @escaping (CMSampleBuffer?, (any Error)?) -> Void
)
```

``` source
optional func loadSampleBufferContainingSamples(to endSampleCursor: (any MESampleCursor)?) async throws -> CMSampleBuffer
```

## Parameters 

`endSampleCursor`  

If not `nil`, this cursor indicates the last sample that the new sample buffer should contain.

`completionHandler`  

The completion block to execute when the load operation finishes.

## Discussion

Plugin format readers that don’t implement sampleLocation() or that always load sample data to answer cursor queries need to implement this method. If a plug-in format reader implements sampleLocation(), implementing loadSampleBufferContainingSamples(to:completionHandler:) is optional.

If there’s no sample data between the sample cursor and `endSampleCursor`, the sample buffer is empty. If an error occurs, the sample buffer is `nil`.

Important

If there’s a change of format description between the sample cursor and `endSampleCursor`, the returned sample buffer needs to contain only the contiguous samples with the same format description as the first sample.

## See Also

### Sending samples to a pipeline

func chunkDetails() throws -> MESampleCursorChunk

Returns information about the chunk that holds the sample indicated by the cursor.

func sampleLocation() throws -> MESampleLocation

Returns the location and byte source of the sample indicated by the cursor.

