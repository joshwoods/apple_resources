

- SwiftUI
- ReferenceFileDocumentConfiguration
-  document 

Instance Property

# document

The current document model.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@ObservedObject @MainActor @preconcurrency
var document: Document { get set }
```

## Discussion

Changes to the document dirty the document state, indicating that it needs to be saved. SwiftUI doesn’t automatically register undo actions.

## See Also

### Getting and setting the document

var $document: ObservedObject&lt;Document>.Wrapper

