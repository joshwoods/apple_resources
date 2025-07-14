

- AVFoundation
- AVSampleBufferGenerator
-  makeSampleBuffer(for:) 

Instance Method

# makeSampleBuffer(for:)

Creates a sample buffer, and attempts to load its data asynchronously if requested.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func makeSampleBuffer(for request: AVSampleBufferRequest) throws -> CMSampleBuffer
```

## Parameters 

`request`  

A sample buffer creation request.

## Return Value

A sample buffer object.

## Discussion

If you created the generator with a `nil` timebase, any associated AVSampleBufferRequest objects default to using a request mode of AVSampleBufferRequest.Mode.immediate.

Call the notifyOfDataReady(for:completionHandler:) class method to have the system notify you when sample buffer data is available.

The request may fail based on generator configuration or file format.

## See Also

### Creating a Sample Buffer

func makeBatch() -> AVSampleBufferGeneratorBatch

Creates a batch object to handle generating multiple sample buffers.

func makeSampleBuffer(for: AVSampleBufferRequest, addTo: AVSampleBufferGeneratorBatch) throws -> CMSampleBuffer

Creates a sample buffer and attempts to defer I/O for its data.

func createSampleBuffer(for: AVSampleBufferRequest) -> CMSampleBuffer?

Creates a new sample buffer reference for the specified buffer request.

Deprecated

