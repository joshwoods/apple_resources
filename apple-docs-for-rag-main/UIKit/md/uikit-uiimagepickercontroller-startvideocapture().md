

- UIKit
- UIImagePickerController
-  startVideoCapture() 

Instance Method

# startVideoCapture()

Starts video capture using the camera specified by the camera device property.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+

``` source
@MainActor
func startVideoCapture() -> Bool
```

## Return Value

true on success or false on failure. This method may return a value of false for various reasons, among them the following:

- Movie capture is already in progress

- The device does not support movie capture

- The device is out of disk space

## Discussion

Use this method in conjunction with a custom overlay view to initiate the programmatic capture of a movie. You can take more than one movie without leaving the interface, but to do so requires you to hide the default image picker controls.

Calling this method while a movie is being captured has no effect. You must call the stopVideoCapture() method, and then wait until the associated delegate object receives an imagePickerController(_:didFinishPickingMediaWithInfo:) message, before you can capture another movie.

Calling this method when the source type of the image picker is set to a value other than UIImagePickerController.SourceType.camera results in the throwing of an invalidArgumentException exception.

If you require additional options or more control over movie capture, use the movie capture methods in the AVFoundation framework. Refer to AVFoundation.

## See Also

### Capturing still images or movies

func takePicture()

Captures a still image using the camera.

func stopVideoCapture()

Stops video capture.

