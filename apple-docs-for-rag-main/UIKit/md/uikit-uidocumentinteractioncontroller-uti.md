

- UIKit
- UIDocumentInteractionController
-  uti 

Instance Property

# uti

The type of the target file.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var uti: String? { get set }
```

## Discussion

The value of this property is used to determine which apps are capable of opening the document. The default value is determined automatically whenever possible. However, if the document is a custom type that cannot be determined readily, the value of this property may be `nil`. If you know the type of the document, you can set the value of this property explicitly.

## See Also

### Accessing the target document’s attributes

var url: URL?

The URL identifying the target file on the local filesystem.

var name: String?

The name of the target file.

var icons: [UIImage]

The images associated with the target file.

var annotation: Any?

Custom property list information for the target file.

