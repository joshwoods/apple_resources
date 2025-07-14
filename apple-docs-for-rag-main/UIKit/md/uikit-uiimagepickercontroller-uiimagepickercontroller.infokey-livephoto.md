

- UIKit
- UIImagePickerController
- UIImagePickerController.InfoKey
-  livePhoto 

Type Property

# livePhoto

The Live Photo representation of the selected or captured photo.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
static let livePhoto: UIImagePickerController.InfoKey
```

## Discussion

A Live Photo is a picture, that includes motion and sound from the moments just before and after its capture. On compatible devices, the Camera app captures all photos as Live Photos by default, but the imagePickerController:didFinishPickingImage:editingInfo: method’s `image` parameter contains only the still image representation.

To obtain the motion and sound content of a live photo for display (using the PHLivePhotoView class), include the `kUTTypeImage` and `kUTTypeLivePhoto` identifiers in the allowed media types when configuring an image picker controller. When the user picks or captures a Live Photo, the `editingInfo` dictionary contains the livePhoto key, with a PHLivePhoto representation of the photo as the corresponding value.

## See Also

### Constants

static let cropRect: UIImagePickerController.InfoKey

The cropping rectangle that was applied to the original image.

static let editedImage: UIImagePickerController.InfoKey

An image edited by the user.

static let imageURL: UIImagePickerController.InfoKey

The URL of the image file.

static let mediaMetadata: UIImagePickerController.InfoKey

Metadata for a newly-captured photograph.

static let mediaType: UIImagePickerController.InfoKey

The media type selected by the user.

static let mediaURL: UIImagePickerController.InfoKey

The filesystem URL for the movie.

static let originalImage: UIImagePickerController.InfoKey

The original, uncropped image selected by the user.

static let phAsset: UIImagePickerController.InfoKey

A Photos asset for the image.

Deprecated

static let referenceURL: UIImagePickerController.InfoKey

The Assets Library URL for the original version of the picked item.

Deprecated

