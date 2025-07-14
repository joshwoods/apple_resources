

- AppKit
- NSTextView
-  changeColor(\_:) 

Instance Method

# changeColor(\_:)

Sets the color of the selected text.

macOS

``` source
@MainActor
func changeColor(_ sender: Any?)
```

## Parameters 

`sender`  

The control that sent the message. `NSTextView`’s implementation sends a color message to `sender` to get the new color.

## See Also

### Setting text attributes

func alignJustified(Any?)

Applies full justification to selected paragraphs (or all text, if the receiver is a plain text object).

func changeAttributes(Any?)

Changes the attributes of the current selection.

func setAlignment(NSTextAlignment, range: NSRange)

Sets the alignment of the paragraphs containing characters in the specified range.

var typingAttributes: [NSAttributedString.Key : Any]

The receiver’s typing attributes.

func useStandardKerning(Any?)

Set the receiver to use pair kerning data for the glyphs in its selection, or for all glyphs if the receiver is a plain text view.

func lowerBaseline(Any?)

Lowers the baseline offset of selected text by 1 point, or of all text if the receiver is a plain text view.

func raiseBaseline(Any?)

Raises the baseline offset of selected text by 1 point, or of all text if the receiver is a plain text view.

func turnOffKerning(Any?)

Sets the receiver to use nominal glyph spacing for the glyphs in its selection, or for all glyphs if the receiver is a plain text view.

func loosenKerning(Any?)

Increases the space between glyphs in the receiver’s selection, or in all text if the receiver is a plain text view.

func tightenKerning(Any?)

Decreases the space between glyphs in the receiver’s selection, or for all glyphs if the receiver is a plain text view.

func useStandardLigatures(Any?)

Sets the receiver to use the standard ligatures available for the fonts and languages used when setting text, for the glyphs in the selection if the receiver is a rich text view, or for all glyphs if it’s a plain text view.

func turnOffLigatures(Any?)

Sets the receiver to use only required ligatures when setting text, for the glyphs in the selection if the receiver is a rich text view, or for all glyphs if it’s a plain text view.

func useAllLigatures(Any?)

Sets the receiver to use all ligatures available for the fonts and languages used when setting text, for the glyphs in the selection if the receiver is a rich text view, or for all glyphs if it’s a plain text view.

func toggleTraditionalCharacterShape(Any?)

Toggles the `NSCharacterShapeAttributeName` attribute at the current selection.

Deprecated

