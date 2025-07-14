

- PDFKit
- PDFPage
-  addAnnotation(\_:) 

Instance Method

# addAnnotation(\_:)

Adds the specified annotation object to the page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func addAnnotation(_ annotation: PDFAnnotation)
```

## See Also

### Working with Annotations

var annotations: [PDFAnnotation]

Returns an array containing the page’s annotations.

var displaysAnnotations: Bool

Returns a Boolean value indicating whether annotations are displayed for the page.

func removeAnnotation(PDFAnnotation)

Removes the specified annotation from the page.

func annotation(at: CGPoint) -> PDFAnnotation?

Returns the annotation, if there is one, at the specified point.

