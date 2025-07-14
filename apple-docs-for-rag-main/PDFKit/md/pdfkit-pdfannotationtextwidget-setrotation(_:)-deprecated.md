

- PDFKit
- PDFAnnotationTextWidget
-  setRotation(\_:) Deprecated

Instance Method

# setRotation(\_:)

Sets the rotation angle of the annotation text field in degrees.

macOS 10.4–10.12Deprecated

``` source
func setRotation(_ rotation: Int32)
```

## Parameters 

`rotation`  

The rotation angle to be applied to the annotation text field, in degrees. The rotation angle must be a positive or negative multiple of 90 (negative angles are converted to their positive equivalents; for example -90 is changed to 270).

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

func rotation() -> Int

Returns the rotation angle of the annotation text field in degrees.

Deprecated

