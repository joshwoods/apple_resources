

- UIKit
- UIImagePickerController
- UIImagePickerController.InfoKey
-  cropRect 

Type Property

# cropRect

The cropping rectangle that was applied to the original image.

iOSiPadOSMac CatalystvisionOS

``` source
static let cropRect: UIImagePickerController.InfoKey
```

## Discussion

The value for this key is an NSValue object containing a CGRect opaque type.

## See Also

### Constants

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

static let referenceURL: UIImagePickerController.InfoKey

The Assets Library URL for the original version of the picked item.

Deprecated

