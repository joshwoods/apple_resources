

- UIKit
- UIImagePickerController
-  availableMediaTypes(for:) 

Type Method

# availableMediaTypes(for:)

Retrieves the available media types for the specified source type.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func availableMediaTypes(for sourceType: UIImagePickerController.SourceType) -> [String]?
```

## Parameters 

`sourceType`  

The source to use to pick an image.

## Return Value

An array whose elements identify the available media types for the specified source type.

## Discussion

Some iOS devices support video recording. Use this method, along with the isSourceTypeAvailable(_:) method, to determine if video recording is available on a device. The availability of video recording is indicated by the presence of the `kUTTypeMovie` media type for the UIImagePickerController.SourceType.camera source type.

## See Also

### Setting the picker source

class func isSourceTypeAvailable(UIImagePickerController.SourceType) -> Bool

Queries whether the device supports picking media using the specified source type.

var sourceType: UIImagePickerController.SourceType

The type of picker interface to be displayed by the controller.

enum SourceType

Constants that describe the source to use when picking an image or when determining available media types.

