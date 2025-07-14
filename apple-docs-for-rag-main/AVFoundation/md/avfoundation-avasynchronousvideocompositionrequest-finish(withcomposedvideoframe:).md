

- AVFoundation
- AVAsynchronousVideoCompositionRequest
-  finish(withComposedVideoFrame:) 

Instance Method

# finish(withComposedVideoFrame:)

Finishes the request to compose the frame.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func finish(withComposedVideoFrame composedVideoFrame: CVPixelBuffer)
```

## Parameters 

`composedVideoFrame`  

The successfully composed pixel buffer.

## Discussion

A custom compositor calls this method to indicate that it’s composed a frame successfully.

## See Also

### Finishing the Request

func finish(with: any Error)

Finishes the request with an error.

func finishCancelledRequest()

Cancels the request to compose a video frame.

