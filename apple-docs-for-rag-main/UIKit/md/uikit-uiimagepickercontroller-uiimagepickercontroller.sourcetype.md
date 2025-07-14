

- UIKit
- UIImagePickerController
-  UIImagePickerController.SourceType 

Enumeration

# UIImagePickerController.SourceType

Constants that describe the source to use when picking an image or when determining available media types.

iOSiPadOSMac CatalystvisionOS

``` source
enum SourceType
```

## Overview

A given source may not be available on a given device because the source is not physically present or because it cannot currently be accessed.

## Topics

### Constants

case camera

Specifies the device’s built-in camera as the source for the image picker controller.

case photoLibrary

Specifies the device’s photo library as the source for the image picker controller.

Deprecated

case savedPhotosAlbum

Specifies the device’s Camera Roll album as the source for the image picker controller.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting the picker source

class func availableMediaTypes(for: UIImagePickerController.SourceType) -> [String]?

Retrieves the available media types for the specified source type.

class func isSourceTypeAvailable(UIImagePickerController.SourceType) -> Bool

Queries whether the device supports picking media using the specified source type.

var sourceType: UIImagePickerController.SourceType

The type of picker interface to be displayed by the controller.

