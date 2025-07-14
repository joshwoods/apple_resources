

- PDFKit
- PDFSelection
-  draw(for:active:) 

Instance Method

# draw(for:active:)

Calls draw(for:with:active:) with a default value for box parameter.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func draw(
    for page: PDFPage,
    active: Bool
)
```

## Discussion

The default value is `kPDFDisplayBoxCropBox`. If active is true, drawing uses `selectedTextBackgroundColor`. If false, it uses `secondarySelectedControlColor`.

## See Also

### Managing Selection Drawing

func draw(for: PDFPage, with: PDFDisplayBox, active: Bool)

Draws the selection relative to the origin of the specified box in page space.

var color: UIColor?

Sets the color used for the drawing of a selection in both active and inactive states.

