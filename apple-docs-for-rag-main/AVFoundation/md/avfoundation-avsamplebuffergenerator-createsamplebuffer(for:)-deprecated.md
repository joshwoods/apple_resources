

- AVFoundation
- AVSampleBufferGenerator
-  createSampleBuffer(for:) Deprecated

Instance Method

# createSampleBuffer(for:)

Creates a new sample buffer reference for the specified buffer request.

macOS 10.10–13.0Deprecated

``` source
func createSampleBuffer(for request: AVSampleBufferRequest) -> CMSampleBuffer?
```

Deprecated

Use -createSampleBufferForRequest: error:, passing NULL for the error if not required

## Parameters 

`request`  

The sample buffer request.

## Return Value

Returns a new `CMSampleBufferRef`.

## Discussion

It is an error to use an `AVSampleBufferRequest` object with mode set to `AVSampleBufferRequestModeScheduled` when the `AVSampleBufferGenerator` was created with a `NULL` timebase.

## See Also

### Creating a Sample Buffer

func makeSampleBuffer(for: AVSampleBufferRequest) throws -> CMSampleBuffer

Creates a sample buffer, and attempts to load its data asynchronously if requested.

func makeBatch() -> AVSampleBufferGeneratorBatch

Creates a batch object to handle generating multiple sample buffers.

func makeSampleBuffer(for: AVSampleBufferRequest, addTo: AVSampleBufferGeneratorBatch) throws -> CMSampleBuffer

Creates a sample buffer and attempts to defer I/O for its data.

