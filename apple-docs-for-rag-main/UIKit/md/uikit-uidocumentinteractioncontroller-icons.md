

- UIKit
- UIDocumentInteractionController
-  icons 

Instance Property

# icons

The images associated with the target file.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var icons: [UIImage] { get }
```

## Discussion

This property contains an array of UIImage objects containing the available icons for the given file. The images in the array are sorted from smallest to largest, with the smallest image located at index 0. The returned array always contains at least one image.

The images themselves are provided by the system and determined by the UTI of the file. Apps can register custom icons for their associated files by including the appropriate meta information in their `Info.plist` file. If no custom icon exists, the images in this property represent the generic document icon.

## See Also

### Accessing the target document’s attributes

var url: URL?

The URL identifying the target file on the local filesystem.

var uti: String?

The type of the target file.

var name: String?

The name of the target file.

var annotation: Any?

Custom property list information for the target file.

