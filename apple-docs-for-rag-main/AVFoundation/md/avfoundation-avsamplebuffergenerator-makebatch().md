

- AVFoundation
- AVSampleBufferGenerator
-  makeBatch() 

Instance Method

# makeBatch()

Creates a batch object to handle generating multiple sample buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func makeBatch() -> AVSampleBufferGeneratorBatch
```

## Return Value

An object to batch generate sample buffers.

## Discussion

Generating sample buffers in batches optimizes performance by allowing the system to asynchronously load sample data and optimize I/O when possible.

## See Also

### Creating a Sample Buffer

func makeSampleBuffer(for: AVSampleBufferRequest) throws -> CMSampleBuffer

Creates a sample buffer, and attempts to load its data asynchronously if requested.

func makeSampleBuffer(for: AVSampleBufferRequest, addTo: AVSampleBufferGeneratorBatch) throws -> CMSampleBuffer

Creates a sample buffer and attempts to defer I/O for its data.

func createSampleBuffer(for: AVSampleBufferRequest) -> CMSampleBuffer?

Creates a new sample buffer reference for the specified buffer request.

Deprecated

