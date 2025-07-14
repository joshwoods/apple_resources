

- PDFKit
- PDFPage
-  annotation(at:) 

Instance Method

# annotation(at:)

Returns the annotation, if there is one, at the specified point.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
func annotation(at point: NSPoint) -> PDFAnnotation?
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func annotation(at point: CGPoint) -> PDFAnnotation?
```

## Discussion

Use this method for hit-testing based on the current cursor position. If more than one annotation shares the specified point, the frontmost (or topmost) one is returned (the annotations are searched in reverse order of their appearance in the PDF data file). Returns `NULL` if there is no annotation at `point`.

Specify the point in page space. Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Working with Annotations

var annotations: [PDFAnnotation]

Returns an array containing the page’s annotations.

var displaysAnnotations: Bool

Returns a Boolean value indicating whether annotations are displayed for the page.

func addAnnotation(PDFAnnotation)

Adds the specified annotation object to the page.

func removeAnnotation(PDFAnnotation)

Removes the specified annotation from the page.

