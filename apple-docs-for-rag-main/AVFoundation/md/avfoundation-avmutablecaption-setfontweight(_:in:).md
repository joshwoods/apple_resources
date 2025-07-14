

- AVFoundation
- AVMutableCaption
-  setFontWeight(\_:in:) 

Instance Method

# setFontWeight(\_:in:)

Sets the font weight for a range of text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func setFontWeight(
    _ fontWeight: AVCaption.FontWeight,
    in range: NSRange
)
```

## Parameters 

`fontWeight`  

The font weight.

`range`  

The range to which this font weight applies.

## See Also

### Configuring Font Styles

enum FontStyle

Font styles for caption text.

func setFontStyle(AVCaption.FontStyle, in: NSRange)

Sets the font style for a range of text.

func removeFontStyle(in: NSRange)

Removes a font style from a range of text.

enum FontWeight

Font weights for a caption.

func removeFontWeight(in: NSRange)

Removes a font weight from a range of text.

struct Decoration

Text decorations for caption text.

func setDecoration(AVCaption.Decoration, in: NSRange)

Sets a decoration for a range of text.

func removeDecoration(in: NSRange)

Removes a decoration from a range of text.

