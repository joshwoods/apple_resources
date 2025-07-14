

- RealityKit
- ObjectCaptureSession
-  startCapturing() 

Instance Method

# startCapturing()

Begins taking images for object capture.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
func startCapturing()
```

## Discussion

This call moves the session state from `.ready` or `.detecting` into `.capturing`. In object-centric scanning, this function is called after the user chooses the object selection bounding box and wishes to start the capture process. This call then moves the session state from `.detecting` into `.capturing`. In freeform scanning where the user skips the bounding box selection, this call moves the session state from `.ready` directly into `.capturing`.

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

func resume()

Resumes object tracking algorithms after pause() is called.

