

- UIKit
- UIImagePickerController
-  takePicture() 

Instance Method

# takePicture()

Captures a still image using the camera.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+

``` source
@MainActor
func takePicture()
```

## Discussion

Use this method in conjunction with a custom overlay view to initiate the programmatic capture of a still image. This supports taking more than one picture without leaving the interface, but requires that you hide the default image picker controls.

Calling this method while an image is being captured has no effect. You must wait until the associated delegate object receives an imagePickerController(_:didFinishPickingMediaWithInfo:) message before you can capture another picture.

Calling this method when the source type of the image picker is set to a value other than UIImagePickerController.SourceType.camera results in the throwing of an invalidArgumentException exception.

## See Also

### Related Documentation

var cameraOverlayView: UIView?

The view to display on top of the default image picker interface.

### Capturing still images or movies

func startVideoCapture() -> Bool

Starts video capture using the camera specified by the camera device property.

func stopVideoCapture()

Stops video capture.

