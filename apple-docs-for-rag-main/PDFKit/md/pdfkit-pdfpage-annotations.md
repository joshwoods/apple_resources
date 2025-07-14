

- PDFKit
- PDFPage
-  annotations 

Instance Property

# annotations

Returns an array containing the page’s annotations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var annotations: [PDFAnnotation] { get }
```

## Discussion

The elements of the array will most likely be typed to subclasses of the PDFAnnotation class.

## See Also

### Working with Annotations

var displaysAnnotations: Bool

Returns a Boolean value indicating whether annotations are displayed for the page.

func addAnnotation(PDFAnnotation)

Adds the specified annotation object to the page.

func removeAnnotation(PDFAnnotation)

Removes the specified annotation from the page.

func annotation(at: CGPoint) -> PDFAnnotation?

Returns the annotation, if there is one, at the specified point.

