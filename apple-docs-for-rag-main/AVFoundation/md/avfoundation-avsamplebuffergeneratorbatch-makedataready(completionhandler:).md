

- AVFoundation
- AVSampleBufferGeneratorBatch
-  makeDataReady(completionHandler:) 

Instance Method

# makeDataReady(completionHandler:)

Loads sample data asynchronously for all sample buffers within a batch.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func makeDataReady(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func makeDataReady() async throws
```

## Parameters 

`completionHandler`  

A callback the system invokes once when all sample buffers in the batch are data-ready, or when an error occurs.

## Discussion

Calling this method more than once on a batch generates an exception.

