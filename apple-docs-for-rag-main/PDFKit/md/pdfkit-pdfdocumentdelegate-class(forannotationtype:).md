

- PDFKit
- PDFDocumentDelegate
-  class(forAnnotationType:) 

Instance Method

# class(forAnnotationType:)

Returns a `PDFAnnotation` subclass for an annotation type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
optional func `class`(forAnnotationType annotationType: String) -> AnyClass
```

## Mentioned in 

Adding Custom Graphics to a PDF

## See Also

### Wrapping Document Elements

func classForPage() -> AnyClass

Returns a `PDFPage` subclass for a page object.

func `class`(forAnnotationClass: AnyClass) -> AnyClass

Returns a `PDFAnnotation` subclass for a class.

Deprecated

