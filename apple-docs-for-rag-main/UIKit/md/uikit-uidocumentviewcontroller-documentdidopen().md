

- UIKit
- UIDocumentViewController
-  documentDidOpen() 

Instance Method

# documentDidOpen()

Provides an opportunity to configure the view after the system loads the controller’s document into memory.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func documentDidOpen()
```

## Mentioned in 

Customizing a document-based app’s launch experience

## Discussion

The system calls this method after the document view controller opens its document, or when an object assigns an already opened document to the document view controller’s `document` property. Override this method to customize the views that present your document in the view:

```
override func documentDidOpen() {
    configureViewForCurrentDocument()
}
```

Configure the view in its own method and call that method in both `documentDidOpen()` and viewDidLoad(). There is no timing guarantee between when the system calls `documentDidOpen` and when it loads the view controller’s view.

## See Also

### Managing the document view

var document: UIDocument?

The document that the controller presents or edits.

func openDocument(completionHandler: (Bool) -> Void)

Opens a document in a document view controller from outside the document view controller.

