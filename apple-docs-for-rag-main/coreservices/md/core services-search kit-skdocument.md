

- Core Services
- Search Kit
-  SKDocument 

Type Alias

# SKDocument

Defines an opaque data type representing a document’s URL.

Mac Catalyst 13.0+macOS 10.3+

``` source
typealias SKDocument = CFTypeRef
```

## Discussion

A document URL object is a generic location specification for a document. It is built from a document scheme, a parent document, and a document name. You can convert back and forth between document URL objects and `CFURL` objects using Search Kit’s SKDocumentCreateWithURL(_:) and SKDocumentCopyURL(_:) functions.

To create a Search Kit document URL object, use SKDocumentCreateWithURL(_:) when you can provide a complete URL, or use SKDocumentCreate(_:_:_:) when you want to specify document location indirectly using a parent document URL object. For other operations on documents, see Working with Documents and Terms.

If you create document URL objects with indirect locations using the SKDocumentCreate(_:_:_:) function, you can resolve the locations by assembling them piece by piece, starting with a document URL object and going up step by step, parent to parent.

