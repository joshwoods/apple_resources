

- PDFKit
- PDFAnnotationTextWidget
-  rotation() Deprecated

Instance Method

# rotation()

Returns the rotation angle of the annotation text field in degrees.

macOS 10.4–10.12Deprecated

``` source
func rotation() -> Int
```

## Return Value

The rotation angle of the annotation text field in degrees.

## Discussion

Note that the rotation value is a positive multiple of 90, such as 0, 90, 180, or 270. The rotation of annotation text fields with negative rotation is converted to a corresponding positive rotation. For example, -90 is changed to 270.

## See Also

### Related Documentation

class PDFAnnotationTextWidget

A `PDFAnnotationTextWidget` object allows you to manage the appearance and content of text fields.

Deprecated

### Managing Background Color, Alignment, and Rotation

func backgroundColor() -> NSColor!

Returns the background color of the annotation text field.

Deprecated

func setBackgroundColor(NSColor!)

Sets the background color of the annotation text field.

Deprecated

func alignment() -> NSTextAlignment

Returns the text alignment setting for the annotation.

Deprecated

func setAlignment(NSTextAlignment)

Sets the text alignment for the annotation.

Deprecated

func setRotation(Int32)

Sets the rotation angle of the annotation text field in degrees.

Deprecated

