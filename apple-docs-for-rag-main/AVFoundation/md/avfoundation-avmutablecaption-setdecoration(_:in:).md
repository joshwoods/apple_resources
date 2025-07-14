

- AVFoundation
- AVMutableCaption
-  setDecoration(\_:in:) 

Instance Method

# setDecoration(\_:in:)

Sets a decoration for a range of text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func setDecoration(
    _ decoration: AVCaption.Decoration,
    in range: NSRange
)
```

## Parameters 

`decoration`  

The decoration.

`range`  

The range to which this decoration applies.

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

func setFontWeight(AVCaption.FontWeight, in: NSRange)

Sets the font weight for a range of text.

func removeFontWeight(in: NSRange)

Removes a font weight from a range of text.

struct Decoration

Text decorations for caption text.

func removeDecoration(in: NSRange)

Removes a decoration from a range of text.

