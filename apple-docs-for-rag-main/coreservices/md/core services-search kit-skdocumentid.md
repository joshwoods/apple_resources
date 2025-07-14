

- Core Services
- Search Kit
-  SKDocumentID 

Type Alias

# SKDocumentID

Defines an opaque data type representing a lightweight document identifier.

Mac Catalyst 13.0+macOS 10.4+

``` source
typealias SKDocumentID = CFIndex
```

## Discussion

Use document IDs rather than document URL objects (SKDocumentRefs) whenever possible. Using document IDs results in faster searching.

You can work with document IDs using a variety of Search Kit functions. See SKIndexGetMaximumDocumentID(_:), SKIndexCopyDocumentForDocumentID(_:_:), SKIndexCopyInfoForDocumentIDs(_:_:_:_:_:), SKIndexCopyDocumentRefsForDocumentIDs(_:_:_:_:), SKIndexCopyDocumentURLsForDocumentIDs(_:_:_:_:), SKIndexCopyDocumentIDArrayForTermID(_:_:), and SKIndexCopyTermIDArrayForDocumentID(_:_:).

