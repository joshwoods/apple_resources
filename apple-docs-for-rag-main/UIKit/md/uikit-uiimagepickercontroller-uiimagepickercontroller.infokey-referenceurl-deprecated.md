

- UIKit
- UIImagePickerController
- UIImagePickerController.InfoKey
-  referenceURL Deprecated

Type Property

# referenceURL

The Assets Library URL for the original version of the picked item.

iOS 4.1–11.0DeprecatediPadOS 4.1–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
static let referenceURL: UIImagePickerController.InfoKey
```

Deprecated

Use PHPickerViewController instead.

## Discussion

After the user edits a picked item—such as by cropping an image or trimming a movie—the URL continues to point to the original version of the picked item.

The value for this key is an NSURL object.

## See Also

### Constants

static let cropRect: UIImagePickerController.InfoKey

The cropping rectangle that was applied to the original image.

static let editedImage: UIImagePickerController.InfoKey

An image edited by the user.

static let imageURL: UIImagePickerController.InfoKey

The URL of the image file.

static let livePhoto: UIImagePickerController.InfoKey

The Live Photo representation of the selected or captured photo.

Deprecated

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

