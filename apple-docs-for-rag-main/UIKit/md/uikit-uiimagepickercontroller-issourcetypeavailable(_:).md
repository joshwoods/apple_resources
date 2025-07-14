

- UIKit
- UIImagePickerController
-  isSourceTypeAvailable(\_:) 

Type Method

# isSourceTypeAvailable(\_:)

Queries whether the device supports picking media using the specified source type.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func isSourceTypeAvailable(_ sourceType: UIImagePickerController.SourceType) -> Bool
```

## Parameters 

`sourceType`  

The source to use to pick an image or movie.

## Return Value

true if the device supports the specified source type; false if the specified source type is not available.

## Discussion

Because a media source may not be present or may be unavailable, devices may not always support all source types. For example, if you attempt to pick an image from the user’s library and the library is empty, this method returns false. Similarly, if the camera is already in use, this method returns false.

Before attempting to use an `UIImagePickerController` object to pick an image, you must call this method to ensure that the desired source type is available.

## See Also

### Setting the picker source

class func availableMediaTypes(for: UIImagePickerController.SourceType) -> [String]?

Retrieves the available media types for the specified source type.

var sourceType: UIImagePickerController.SourceType

The type of picker interface to be displayed by the controller.

enum SourceType

Constants that describe the source to use when picking an image or when determining available media types.

