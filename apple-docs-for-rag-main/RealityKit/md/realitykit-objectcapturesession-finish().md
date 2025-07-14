

- RealityKit
- ObjectCaptureSession
-  finish() 

Instance Method

# finish()

Requests that the capture session be stopped and all data saved.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
func finish()
```

## Discussion

Call this method when the user has completed the scan successfully. The session switches to state `.finishing` while it saves all data and ultimately switches the state to `.completed`. The session ignores this method call if the current state is any value other than `.capturing`.

## See Also

### Controlling the session

func cancel()

Requests that the capture session be canceled.

func pause()

Pauses the automatic capture and other resource-intense algorithms.

func requestImageCapture()

Requests a manual image capture.

func resume()

Resumes object tracking algorithms after pause() is called.

func startCapturing()

Begins taking images for object capture.

