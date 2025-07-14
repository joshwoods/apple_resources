

- UIKit
- UIDocumentViewController
-  openDocument(completionHandler:) 

Instance Method

# openDocument(completionHandler:)

Opens a document in a document view controller from outside the document view controller.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
func openDocument(completionHandler: @escaping (Bool) -> Void)
```

``` source
@MainActor
func openDocument() async -> Bool
```

## Parameters 

`completionHandler`  

The function that executes after the document view controller opens the document

## See Also

### Managing the document view

var document: UIDocument?

The document that the controller presents or edits.

func documentDidOpen()

Provides an opportunity to configure the view after the system loads the controller’s document into memory.

