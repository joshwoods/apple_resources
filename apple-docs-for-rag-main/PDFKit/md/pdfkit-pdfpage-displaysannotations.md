

- PDFKit
- PDFPage
-  displaysAnnotations 

Instance Property

# displaysAnnotations

Returns a Boolean value indicating whether annotations are displayed for the page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var displaysAnnotations: Bool { get set }
```

## Discussion

If true, the page will draw annotations when a drawing method is called.

## See Also

### Related Documentation

func draw(with: PDFDisplayBox)

Draws the page within the specified box.

Deprecated

### Working with Annotations

var annotations: [PDFAnnotation]

Returns an array containing the page’s annotations.

func addAnnotation(PDFAnnotation)

Adds the specified annotation object to the page.

func removeAnnotation(PDFAnnotation)

Removes the specified annotation from the page.

func annotation(at: CGPoint) -> PDFAnnotation?

Returns the annotation, if there is one, at the specified point.

