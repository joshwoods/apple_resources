

- PDFKit
- PDFDocumentDelegate
-  class(forAnnotationClass:) Deprecated

Instance Method

# class(forAnnotationClass:)

Returns a `PDFAnnotation` subclass for a class.

macOS 10.6–10.12Deprecated

``` source
optional func `class`(forAnnotationClass annotationClass: AnyClass) -> AnyClass
```

## See Also

### Wrapping Document Elements

func classForPage() -> AnyClass

Returns a `PDFPage` subclass for a page object.

func `class`(forAnnotationType: String) -> AnyClass

Returns a `PDFAnnotation` subclass for an annotation type.

