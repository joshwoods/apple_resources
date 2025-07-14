

- UIKit
- UIDocumentInteractionController
-  name 

Instance Property

# name

The name of the target file.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var name: String? { get set }
```

## Discussion

This property contains the filename without any preceding path information. The default value of this property is derived from the path information in the url property. You can change the value of this property as needed if you want to associate a different name with the file.

## See Also

### Accessing the target document’s attributes

var url: URL?

The URL identifying the target file on the local filesystem.

var uti: String?

The type of the target file.

var icons: [UIImage]

The images associated with the target file.

var annotation: Any?

Custom property list information for the target file.

