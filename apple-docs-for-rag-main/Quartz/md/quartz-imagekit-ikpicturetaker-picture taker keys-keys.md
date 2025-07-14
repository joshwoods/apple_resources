

- Quartz
- ImageKit
- IKPictureTaker
-  Picture Taker Keys 

API Collection

# Picture Taker Keys

Keys for customizing the picture taker appearance and behavior. These values are set by sending the picture taker instance `setValue:forKey`.

## Topics

### Constants

let IKPictureTakerAllowsVideoCaptureKey: String

A key for allowing video capture.

let IKPictureTakerAllowsFileChoosingKey: String

A key for allowing the user to choose a file.

let IKPictureTakerUpdateRecentPictureKey: String

A key for allowing a recent picture to be updated.

let IKPictureTakerAllowsEditingKey: String

A key for allowing image editing.

let IKPictureTakerShowEffectsKey: String

A key for showing effects.

let IKPictureTakerInformationalTextKey: String

A key for informational text. The associated value is an `NSString` or `NSAttributedString` object whose default value is `"Drag Image Here"`.

let IKPictureTakerImageTransformsKey: String

A n image transformation key. The associated value is an `NSDictionary` object that can be serialized.

let IKPictureTakerOutputImageMaxSizeKey: String

A key for the maximum size of the output image. The associated value is an `NSValue` object (`NSSize`).

let IKPictureTakerCropAreaSizeKey: String

A key for the cropping area size. The associated value is an `NSValue` object (`NSSize`).

Deprecated

let IKPictureTakerShowAddressBookPictureKey: String

A key for showing the address book picture.

let IKPictureTakerShowEmptyPictureKey: String

A key for showing an empty picture. The associated value is an `NSImage` object. The default value is `nil`. If set to an image, the picture taker automatically shows an image at the end of the Recent Pictures pop-up menu. that means “no picture.”

let IKPictureTakerRemainOpenAfterValidateKey: String

A key that determines if the picture taker UI should remain open after the user selects done.

