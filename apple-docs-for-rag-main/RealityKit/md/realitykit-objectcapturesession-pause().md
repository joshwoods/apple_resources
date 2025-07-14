

- RealityKit
- ObjectCaptureSession
-  pause() 

Instance Method

# pause()

Pauses the automatic capture and other resource-intense algorithms.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
func pause()
```

## Discussion

Call this when object capture view is not visible, such as when a help screen is shown.

## See Also

### Controlling the session

func cancel()

Requests that the capture session be canceled.

func finish()

Requests that the capture session be stopped and all data saved.

func requestImageCapture()

Requests a manual image capture.

func resume()

Resumes object tracking algorithms after pause() is called.

func startCapturing()

Begins taking images for object capture.

