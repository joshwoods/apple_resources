

- PDFKit
- PDFPage
-  removeAnnotation(\_:) 

Instance Method

# removeAnnotation(\_:)

Removes the specified annotation from the page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func removeAnnotation(_ annotation: PDFAnnotation)
```

## See Also

### Working with Annotations

var annotations: [PDFAnnotation]

Returns an array containing the page’s annotations.

var displaysAnnotations: Bool

Returns a Boolean value indicating whether annotations are displayed for the page.

func addAnnotation(PDFAnnotation)

Adds the specified annotation object to the page.

func annotation(at: CGPoint) -> PDFAnnotation?

Returns the annotation, if there is one, at the specified point.

