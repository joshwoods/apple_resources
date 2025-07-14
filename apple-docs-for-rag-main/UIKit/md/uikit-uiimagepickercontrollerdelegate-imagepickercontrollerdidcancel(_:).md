

- UIKit
- UIImagePickerControllerDelegate
-  imagePickerControllerDidCancel(\_:) 

Instance Method

# imagePickerControllerDidCancel(\_:)

Tells the delegate that the user canceled the pick operation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func imagePickerControllerDidCancel(_ picker: UIImagePickerController)
```

## Parameters 

`picker`  

The controller object managing the image picker interface.

## Discussion

Your delegate’s implementation of this method should dismiss the picker view by calling the dismiss(animated:completion:) method of the parent view controller.

Implementation of this method is optional, but expected.

## See Also

### Closing the picker

func imagePickerController(UIImagePickerController, didFinishPickingMediaWithInfo: [UIImagePickerController.InfoKey : Any])

Tells the delegate that the user picked a still image or movie.

