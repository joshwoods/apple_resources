

- UIKit
- UIDocument
-  documentState 

Instance Property

# documentState

The current state of the document.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var documentState: UIDocument.State { get }
```

## Discussion

When document state changes, the UIDocument object stores a constant identifying the new state in this property. See the UIDocument.State enum for descriptions of these constants. To receive notifications about changes in document state, observe the stateChangedNotification notification.

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

var progress: Progress?

The upload or download progress of a document.

