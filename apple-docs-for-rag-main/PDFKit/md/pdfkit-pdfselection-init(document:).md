

- PDFKit
- PDFSelection
-  init(document:) 

Initializer

# init(document:)

Returns an empty `PDFSelection` object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
init(document: PDFDocument)
```

## Discussion

Typically, you don’t need to create a `PDFSelection` object, but you can use an empty `PDFSelection` object as a container into which you can place selections, using PDFSelection and addSelections.

