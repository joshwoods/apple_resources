

- UIKit
- UIDocumentViewController
-  init(document:) 

Initializer

# init(document:)

Creates a document view controller with a document.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
init(document: UIDocument?)
```

## Parameters 

`document`  

The document that the view controller presents.

## Return Value

A newly initialized UIDocumentViewController object.

## Discussion

The document view controller opens and displays the document that you specify. If you don’t provide custom values, the new view controller gets its title and other information from the document itself.

