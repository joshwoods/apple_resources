

- PDFKit
- PDFDocument
-  allowsDocumentChanges 

Instance Property

# allowsDocumentChanges

A Boolean value indicating whether you can modify the document contents except for document attributes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var allowsDocumentChanges: Bool { get }
```

## See Also

### Getting Permissions

var allowsCopying: Bool

A Boolean value indicating whether the document allows copying of content to the Pasteboard.

var allowsPrinting: Bool

A Boolean value indicating whether the document allows printing.

var allowsCommenting: Bool

A Boolean value indicating whether you can create or modify document annotations, including form field entries.

var allowsContentAccessibility: Bool

A Boolean value indicating whether you can extract content from the document, but only for the purpose of accessibility.

var allowsDocumentAssembly: Bool

A Boolean value indicating whether you can manage a document by inserting, deleting, and rotating pages.

var allowsFormFieldEntry: Bool

A Boolean value indicating whether you can modify form field entries even if you can’t edit document annotations.

