

- UIKit
- UIImagePickerController
-  cameraViewTransform 

Instance Property

# cameraViewTransform

The transform to apply to the camera’s preview image.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+

``` source
@MainActor
var cameraViewTransform: CGAffineTransform { get set }
```

## Discussion

This transform affects the live preview image only and does not affect your custom overlay view or the default image picker controls. You can use this property in conjunction with custom controls to implement your own electronic zoom behaviors.

You can access this property only when the source type of the image picker is set to UIImagePickerController.SourceType.camera. Attempting to access this property for other source types results in the throwing of an invalidArgumentException exception.

## See Also

### Customizing the camera controls

Customizing an image picker controller

Manage user interactions and present custom information when taking pictures by adding an overlay view to your image picker.

var showsCameraControls: Bool

A Boolean value that indicates whether the image picker displays the default camera controls.

var cameraOverlayView: UIView?

The view to display on top of the default image picker interface.

