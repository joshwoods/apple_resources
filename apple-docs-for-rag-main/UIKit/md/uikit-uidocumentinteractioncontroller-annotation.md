

- UIKit
- UIDocumentInteractionController
-  annotation 

Instance Property

# annotation

Custom property list information for the target file.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var annotation: Any? { get set }
```

## Discussion

Use this property to pass information about the document type to the app responsible for opening it. Although the type of this object should be one used to contain property list information—namely, NSDictionary, NSArray, NSData, NSString, NSNumber, or NSDate—the root object must be an NSDictionary.

## See Also

### Accessing the target document’s attributes

var url: URL?

The URL identifying the target file on the local filesystem.

var uti: String?

The type of the target file.

var name: String?

The name of the target file.

var icons: [UIImage]

The images associated with the target file.

