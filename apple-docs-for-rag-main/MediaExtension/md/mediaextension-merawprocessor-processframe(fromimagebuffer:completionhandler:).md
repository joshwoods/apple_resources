

- MediaExtension
- MERAWProcessor
-  processFrame(fromImageBuffer:completionHandler:) 

Instance Method

# processFrame(fromImageBuffer:completionHandler:)

Requests the processor to process a video frame.

macOS 15.0+

``` source
func processFrame(
    fromImageBuffer inputFrame: CVPixelBuffer,
    completionHandler: @escaping (CVPixelBuffer?, (any Error)?) -> Void
)
```

``` source
func processFrame(fromImageBuffer inputFrame: CVPixelBuffer) async throws -> CVPixelBuffer
```

**Required**

## Parameters 

`inputFrame`  

A CVPixelBuffer that contains a video frame to process.

`completionHandler`  

The handler is invoked when a frame processes and is ready to be sent back to the caller. This block does not need to be called in the order in which frames were submitted.

## Discussion

The completionHandler block must be called for every processFrame(fromImageBuffer:completionHandler:) call when processing is complete. The completion handler block should return either a processed pixel buffer or an error.

