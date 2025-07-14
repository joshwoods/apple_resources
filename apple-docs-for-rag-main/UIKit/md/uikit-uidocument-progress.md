

- UIKit
- UIDocument
-  progress 

Instance Property

# progress

The upload or download progress of a document.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var progress: Progress? { get }
```

## Discussion

The value of this property is valid while progressAvailable is set.

## See Also

### Accessing document attributes

var fileURL: URL

The file URL you use to initialize the document.

var localizedName: String

The localized name of the document.

var fileType: String?

The file type of the document.

var fileModificationDate: Date?

The date and time your app last modified the document file.

var documentState: UIDocument.State

The current state of the document.

