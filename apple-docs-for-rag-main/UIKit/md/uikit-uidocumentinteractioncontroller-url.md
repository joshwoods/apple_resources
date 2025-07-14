

- UIKit
- UIDocumentInteractionController
-  url 

Instance Property

# url

The URL identifying the target file on the local filesystem.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var url: URL? { get set }
```

## See Also

### Accessing the target document’s attributes

var uti: String?

The type of the target file.

var name: String?

The name of the target file.

var icons: [UIImage]

The images associated with the target file.

var annotation: Any?

Custom property list information for the target file.

