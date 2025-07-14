

- UIKit
-  UIImagePickerControllerDelegate 

Protocol

# UIImagePickerControllerDelegate

A set of methods that your delegate object must implement to interact with the image picker interface.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UIImagePickerControllerDelegate : NSObjectProtocol
```

## Overview

The methods of this protocol notify your delegate when the user either picks an image or movie, or cancels the picker operation. The delegate methods are responsible for dismissing the picker when the operation completes. To dismiss the picker, call the dismiss(animated:completion:) method of the parent controller responsible for displaying the UIImagePickerController object.

To save a still image to the user’s Camera Roll album, call the UIImageWriteToSavedPhotosAlbum(_:_:_:_:) function from within the body of the imagePickerController(_:didFinishPickingMediaWithInfo:) method. To save a movie to the user’s Camera Roll album, instead call the UISaveVideoAtPathToSavedPhotosAlbum(_:_:_:_:) function. These functions, described in `UIKit Functions`, save the image or movie only; they don’t save metadata.

To write additional metadata when saving an image to the Camera Roll, use the PHAssetChangeRequest class from the Photos framework. See the description for the mediaMetadata key.

## Topics

### Closing the picker

func imagePickerController(UIImagePickerController, didFinishPickingMediaWithInfo: [UIImagePickerController.InfoKey : Any])

Tells the delegate that the user picked a still image or movie.

func imagePickerControllerDidCancel(UIImagePickerController)

Tells the delegate that the user canceled the pick operation.

### Getting the editing information

struct InfoKey

Keys you use to retrieve information from the editing dictionary about the media that the user selected.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to interactions with the picker

var delegate: (any UIImagePickerControllerDelegate &amp; UINavigationControllerDelegate)?

The image picker’s delegate object.

