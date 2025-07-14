

- UIKit
- UIImagePickerController
-  allowsEditing 

Instance Property

# allowsEditing

A Boolean value that indicates whether the user is allowed to edit a selected still image or movie.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsEditing: Bool { get set }
```

## Discussion

If you allow the user to edit still images or movies, the delegate may receive a dictionary with information about the edits that were made. The protocol for the delegate is described in UIImagePickerControllerDelegate.

This property is set to false by default.

## See Also

### Configuring the picker

var mediaTypes: [String]

An array that indicates the media types to access by the media picker controller.

