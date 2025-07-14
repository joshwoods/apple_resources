

- PDFKit
- PDFDocumentDelegate
-  classForPage() 

Instance Method

# classForPage()

Returns a `PDFPage` subclass for a page object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
optional func classForPage() -> AnyClass
```

## Mentioned in 

Adding Custom Graphics to a PDF

## See Also

### Wrapping Document Elements

func `class`(forAnnotationClass: AnyClass) -> AnyClass

Returns a `PDFAnnotation` subclass for a class.

Deprecated

func `class`(forAnnotationType: String) -> AnyClass

Returns a `PDFAnnotation` subclass for an annotation type.

