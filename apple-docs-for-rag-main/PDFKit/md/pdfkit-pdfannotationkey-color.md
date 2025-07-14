

- PDFKit
- PDFAnnotationKey
-  color 

Type Property

# color

An array of floats or a color object that specifies the annotation’s color.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let color: PDFAnnotationKey
```

## Discussion

Annotations use the color for the following:

- The background of the annotation’s icon when it’s in a closed state

- The title bar of the annotation’s pop-up window

- The border of a link annotation

- The stroke of a circle, square, or line shape annotation

## See Also

### Configuring Annotation Appearance

static let appearanceDictionary: PDFAnnotationKey

A dictionary that contains properties for controlling the annotation’s visual appearance.

static let appearanceState: PDFAnnotationKey

A string that specifies the appearance stream for the annotation.

static let border: PDFAnnotationKey

An array of integers or border objects that describes the border of the annotation.

static let borderStyle: PDFAnnotationKey

A dictionary that contains the properties of the annotation’s border.

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

