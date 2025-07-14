

- AVFoundation
- AVSampleBufferGeneratorBatch
-  cancel() 

Instance Method

# cancel()

Cancels any I/O for this batch.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func cancel()
```

## Discussion

The system invokes the associated sample buffers data ready handlers with an error.

