

- UIKit
- UIImagePickerController
- UIImagePickerController.InfoKey
-  mediaMetadata 

Type Property

# mediaMetadata

Metadata for a newly-captured photograph.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
static let mediaMetadata: UIImagePickerController.InfoKey
```

## Discussion

This key is valid only when using an image picker whose source type is set to UIImagePickerController.SourceType.camera, and applies only to still images.

The value for this key is an NSDictionary object that contains the metadata of the photo that was just captured. To store the metadata along with the image in the Camera Roll, use the PHAssetChangeRequest class from the Photos framework.

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

