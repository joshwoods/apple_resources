

- UIKit
- UIDocumentViewController
-  document 

Instance Property

# document

The document that the controller presents or edits.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
var document: UIDocument? { get set }
```

## Discussion

This property represents the document that the document view controller displays. The default value of this property is `nil`. When the value of the `document` property is `nil`, the document view controller presents an empty state view with a message to “Select a document by tapping the ‘Documents’ button at the top.”

When the value of this property is not `nil`, the document view controller displays the document.

## See Also

### Managing the document view

func openDocument(completionHandler: (Bool) -> Void)

Opens a document in a document view controller from outside the document view controller.

func documentDidOpen()

Provides an opportunity to configure the view after the system loads the controller’s document into memory.

