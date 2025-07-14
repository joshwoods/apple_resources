

- PDFKit
- PDFAnnotationKey
-  appearanceDictionary 

Type Property

# appearanceDictionary

A dictionary that contains properties for controlling the annotation’s visual appearance.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let appearanceDictionary: PDFAnnotationKey
```

## Discussion

PDFKit typically generates this property when saving a PDF document. If present, PDFKit uses the contents of the dictionary to render the annotation. PDFKit clears this value if either of the following occurs:

- The appearance changes and PDFKit must rerender the annotation, such as if the color changes.

- Explicit removal of the value occurs to allow use of the annotation’s properties for rendering.

## See Also

### Configuring Annotation Appearance

static let appearanceState: PDFAnnotationKey

A string that specifies the appearance stream for the annotation.

static let border: PDFAnnotationKey

An array of integers or border objects that describes the border of the annotation.

static let borderStyle: PDFAnnotationKey

A dictionary that contains the properties of the annotation’s border.

static let color: PDFAnnotationKey

An array of floats or a color object that specifies the annotation’s color.

static let defaultAppearance: PDFAnnotationKey

A string value a free text annotation uses to format the text.

static let highlightingMode: PDFAnnotationKey

A string value that defines the way an annotation highlights when the user activates it, such as when clicking or tapping a link.

struct PDFAnnotationHighlightingMode

static let iconName: PDFAnnotationKey

A string value that specifies the name of an icon for a text or stamp annotation.

static let interiorColor: PDFAnnotationKey

An array of floating point values or a PDF color object that annotations use to fill interior space, such as line endings, squares, or circles.

static let quadding: PDFAnnotationKey

An integer value that specifies left, right, or center justification.

