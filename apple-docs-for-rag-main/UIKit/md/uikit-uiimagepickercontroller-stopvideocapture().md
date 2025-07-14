

- UIKit
- UIImagePickerController
-  stopVideoCapture() 

Instance Method

# stopVideoCapture()

Stops video capture.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
@MainActor
func stopVideoCapture()
```

## Discussion

After you call this method to stop video capture, the system calls the image picker delegate’s imagePickerController(_:didFinishPickingMediaWithInfo:) method.

## See Also

### Capturing still images or movies

func takePicture()

Captures a still image using the camera.

func startVideoCapture() -> Bool

Starts video capture using the camera specified by the camera device property.

