

- AVFoundation
- AVAsynchronousVideoCompositionRequest
-  finish(with:) 

Instance Method

# finish(with:)

Finishes the request with an error.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func finish(with error: any Error)
```

## Parameters 

`error`  

Returns the error encountered during the compositing.

## Discussion

A custom compositor calls this method to indicate that the attempt to compose a frame failed.

## See Also

### Finishing the Request

func finish(withComposedVideoFrame: CVPixelBuffer)

Finishes the request to compose the frame.

func finishCancelledRequest()

Cancels the request to compose a video frame.

