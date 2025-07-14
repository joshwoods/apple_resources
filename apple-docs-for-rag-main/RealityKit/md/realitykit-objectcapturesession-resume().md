

- RealityKit
- ObjectCaptureSession
-  resume() 

Instance Method

# resume()

Resumes object tracking algorithms after pause() is called.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
func resume()
```

## Discussion

Call this method when the object capture view first appears on the screen, or after `pause()` is called to show another view temporarily.

## See Also

### Controlling the session

func cancel()

Requests that the capture session be canceled.

func finish()

Requests that the capture session be stopped and all data saved.

func pause()

Pauses the automatic capture and other resource-intense algorithms.

func requestImageCapture()

Requests a manual image capture.

func startCapturing()

Begins taking images for object capture.

