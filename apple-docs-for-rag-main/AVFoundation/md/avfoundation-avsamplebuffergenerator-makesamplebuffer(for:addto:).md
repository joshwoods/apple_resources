

- AVFoundation
- AVSampleBufferGenerator
-  makeSampleBuffer(for:addTo:) 

Instance Method

# makeSampleBuffer(for:addTo:)

Creates a sample buffer and attempts to defer I/O for its data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func makeSampleBuffer(
    for request: AVSampleBufferRequest,
    addTo batch: AVSampleBufferGeneratorBatch
) throws -> CMSampleBuffer
```

## Parameters 

`request`  

A sample buffer creation request.

`batch`  

A batch object to contain the output sample buffer. You must create this object by calling makeBatch() on the same instance of AVSampleBufferGenerator or an error occurs.

## Return Value

A sample buffer.

## Discussion

Call the makeDataReady(completionHandler:) on AVSampleBufferGeneratorBatch once to commence I/O and load sample data for all CMSampleBuffer objects in a batch. After loading commences, any subsequent calls to makeSampleBuffer(for:addTo:) throw an exception.

The generator may defer I/O to fetch sample data depending on the source of the sample data and the generator’s timebase

The request may fail based on generator configuration or file format.

## See Also

### Creating a Sample Buffer

func makeSampleBuffer(for: AVSampleBufferRequest) throws -> CMSampleBuffer

Creates a sample buffer, and attempts to load its data asynchronously if requested.

func makeBatch() -> AVSampleBufferGeneratorBatch

Creates a batch object to handle generating multiple sample buffers.

func createSampleBuffer(for: AVSampleBufferRequest) -> CMSampleBuffer?

Creates a new sample buffer reference for the specified buffer request.

Deprecated

