

- RealityKit
- ObjectCaptureSession
-  cancel() 

Instance Method

# cancel()

Requests that the capture session be canceled.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
func cancel()
```

## Discussion

Call this when the user indicates they want to cancel the scan. Calling this method eventually transitions the session to `.failed(Error)` Once the session enters the failed state it is safe to tear down the session and create a new one if desired.

## See Also

### Controlling the session

func finish()

Requests that the capture session be stopped and all data saved.

func pause()

Pauses the automatic capture and other resource-intense algorithms.

func requestImageCapture()

Requests a manual image capture.

func resume()

Resumes object tracking algorithms after pause() is called.

func startCapturing()

Begins taking images for object capture.

