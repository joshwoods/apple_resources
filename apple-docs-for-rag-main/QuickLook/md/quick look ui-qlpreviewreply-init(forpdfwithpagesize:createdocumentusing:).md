

- Quick Look UI
- QLPreviewReply
-  init(forPDFWithPageSize:createDocumentUsing:) 

Initializer

# init(forPDFWithPageSize:createDocumentUsing:)

macOS 12.0+

``` source
convenience init(
    forPDFWithPageSize defaultPageSize: CGSize,
    createDocumentUsing closure: @escaping (QLPreviewReply) throws -> PDFDocument
)
```

