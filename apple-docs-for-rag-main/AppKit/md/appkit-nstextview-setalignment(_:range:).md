

- AppKit
- NSTextView
-  setAlignment(\_:range:) 

Instance Method

# setAlignment(\_:range:)

Sets the alignment of the paragraphs containing characters in the specified range.

macOS

``` source
@MainActor
func setAlignment(
    _ alignment: NSTextAlignment,
    range: NSRange
)
```

## Parameters 

`alignment`  

The new alignment.

`range`  

The range of characters whose paragraphs will have their alignment set.

## Discussion

This method does not include undo support by default. Clients must invoke shouldChangeText(inRanges:replacementStrings:) or shouldChangeText(in:replacementString:) to include this method in an undoable action.

## See Also

### Related Documentation

var rangeForUserParagraphAttributeChange: NSRange

The range of characters affected by an action method that changes paragraph (not character) attributes.

### Setting text attributes

func alignJustified(Any?)

Applies full justification to selected paragraphs (or all text, if the receiver is a plain text object).

func changeAttributes(Any?)

Changes the attributes of the current selection.

func changeColor(Any?)

Sets the color of the selected text.

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

