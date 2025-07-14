

- PDFKit
- PDFPage
-  setBounds(\_:for:) 

Instance Method

# setBounds(\_:for:)

Sets the bounds for the specified box.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func setBounds(
    _ bounds: CGRect,
    for box: PDFDisplayBox
)
```

**macOS**

``` source
func setBounds(
    _ bounds: NSRect,
    for box: PDFDisplayBox
)
```

## Discussion

If the box does not exist, this method creates it for you.

To remove a box, pass `NSZeroRect` for the bounds (note that you cannot remove the media box). If the box bounds are not in range, this method throws a range exception.

## See Also

### Getting Information About a Page

var document: PDFDocument?

Returns the `PDFDocument` object with which the page is associated.

var label: String?

Returns the label for the page.

func bounds(for: PDFDisplayBox) -> CGRect

Returns the bounds for the specified PDF display box.

var rotation: Int

Sets the rotation angle for the page in degrees.

