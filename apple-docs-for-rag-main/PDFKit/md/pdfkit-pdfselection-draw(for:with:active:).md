

- PDFKit
- PDFSelection
-  draw(for:with:active:) 

Instance Method

# draw(for:with:active:)

Draws the selection relative to the origin of the specified box in page space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func draw(
    for page: PDFPage,
    with box: PDFDisplayBox,
    active: Bool
)
```

## Discussion

The selection is drawn using the current highlight color. If active is true, drawing uses `selectedTextBackgroundColor`. If false, it uses `secondarySelectedControlColor`. Refer to the PDFPage class for the list of available box types.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Managing Selection Drawing

func draw(for: PDFPage, active: Bool)

Calls draw(for:with:active:) with a default value for box parameter.

var color: UIColor?

Sets the color used for the drawing of a selection in both active and inactive states.

