

- UIKit
- UIDocument
-  localizedName 

Instance Property

# localizedName

The localized name of the document.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var localizedName: String { get }
```

## Discussion

By default, UIKit obtains the value from the filename component of fileURL. You can override the getter accessor method of this property to provide a custom name for presentation to the user, such as in error strings. See UIDocument for overriding advice.

UIKit sets this property before it calls the completion handlers of the open(completionHandler:), save(to:for:completionHandler:), and revert(toContentsOf:completionHandler:). If, outside of these methods or their completion handlers, you want to wait for any pending file operations to complete before you access this property, you can call performAsynchronousFileAccess(_:) and access the property value in the block parameter.

## See Also

### Accessing document attributes

var fileURL: URL

The file URL you use to initialize the document.

var fileType: String?

The file type of the document.

var fileModificationDate: Date?

The date and time your app last modified the document file.

var documentState: UIDocument.State

The current state of the document.

var progress: Progress?

The upload or download progress of a document.

