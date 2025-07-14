

- RealityKit
- ObjectCaptureSession
-  requestImageCapture() 

Instance Method

# requestImageCapture()

Requests a manual image capture.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
func requestImageCapture()
```

## Discussion

If the session’s state is `.capturing`, call this method to request an image be manually captured at the current location. This function has no effect if the session is in any other state, or if canRequestImageCapture is `false`.

## See Also

### Controlling the session

func cancel()

Requests that the capture session be canceled.

func finish()

Requests that the capture session be stopped and all data saved.

func pause()

Pauses the automatic capture and other resource-intense algorithms.

func resume()

Resumes object tracking algorithms after pause() is called.

func startCapturing()

Begins taking images for object capture.

