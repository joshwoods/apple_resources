

- AVFoundation
- AVMutableCaption
-  setFontStyle(\_:in:) 

Instance Method

# setFontStyle(\_:in:)

Sets the font style for a range of text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func setFontStyle(
    _ fontStyle: AVCaption.FontStyle,
    in range: NSRange
)
```

## Parameters 

`fontStyle`  

The font style.

`range`  

The range to which this style applies.

## See Also

### Configuring Font Styles

enum FontStyle

Font styles for caption text.

func removeFontStyle(in: NSRange)

Removes a font style from a range of text.

enum FontWeight

Font weights for a caption.

func setFontWeight(AVCaption.FontWeight, in: NSRange)

Sets the font weight for a range of text.

func removeFontWeight(in: NSRange)

Removes a font weight from a range of text.

struct Decoration

Text decorations for caption text.

func setDecoration(AVCaption.Decoration, in: NSRange)

Sets a decoration for a range of text.

func removeDecoration(in: NSRange)

Removes a decoration from a range of text.

