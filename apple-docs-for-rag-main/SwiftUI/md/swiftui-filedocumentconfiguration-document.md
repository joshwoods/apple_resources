

- SwiftUI
- FileDocumentConfiguration
-  document 

Instance Property

# document

The current document model.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@Binding
var document: Document { get nonmutating set }
```

## Discussion

Setting a new value marks the document as having changes for later saving and registers an undo action to restore the model to its previous value.

If isEditable is `false`, setting a new value has no effect because the document is in viewing mode.

## See Also

### Getting and setting the document

var $document: Binding&lt;Document>

