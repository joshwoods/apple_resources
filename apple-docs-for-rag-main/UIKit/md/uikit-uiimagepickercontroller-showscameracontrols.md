

- UIKit
- UIImagePickerController
-  showsCameraControls 

Instance Property

# showsCameraControls

A Boolean value that indicates whether the image picker displays the default camera controls.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+

``` source
@MainActor
var showsCameraControls: Bool { get set }
```

## Discussion

The default value of this property is true, which specifies that the default camera controls are visible in the picker. Set it to false to hide the default controls if you want to instead provide a custom overlay view using the cameraOverlayView property.

Note

In iOS 3.1.3 and earlier, hiding the default camera controls limits you to taking still pictures only, regardless of whether movie capture is available on the device.

If you set this property to false and provide your own custom controls, you can take multiple pictures before dismissing the image picker interface. However, if you set this property to true, your delegate must dismiss the image picker interface after the user takes one picture or cancels the operation.

You can access this property only when the source type of the image picker is set to UIImagePickerController.SourceType.camera. Attempting to access this property for other source types results in the throwing of an invalidArgumentException exception. Depending on the value you assign to the mediaTypes property, the default controls display the still camera or movie camera interface, or a selection control that lets the user choose the picker interface.

## See Also

### Related Documentation

func takePicture()

Captures a still image using the camera.

### Customizing the camera controls

Customizing an image picker controller

Manage user interactions and present custom information when taking pictures by adding an overlay view to your image picker.

var cameraOverlayView: UIView?

The view to display on top of the default image picker interface.

var cameraViewTransform: CGAffineTransform

The transform to apply to the camera’s preview image.

