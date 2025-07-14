

- AppKit
- NSForm
-  setTitleBaseWritingDirection(\_:) Deprecated

Instance Method

# setTitleBaseWritingDirection(\_:)

Sets the writing direction for the title of every control embedded in the form.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func setTitleBaseWritingDirection(_ writingDirection: NSWritingDirection)
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`writingDirection`  

This value can be one of the following constants: `NSWritingDirectionNatural`, `NSWritingDirectionLeftToRight`, or `NSWritingDirectionRightToLeft`.

## See Also

### Changing the Appearance of All the Entries

func setBezeled(Bool)

Sets whether the receiver’s entries should display a bezel around their editable text.

Deprecated

func setBordered(Bool)

Sets whether the receiver’s entries should display a border around their editable text fields.

Deprecated

func setEntryWidth(CGFloat)

Sets the width of all the entries in the receiver.

Deprecated

func setFrameSize(NSSize)

Sets the size of the receiver’s frame size to the specified value.

Deprecated

func setInterlineSpacing(CGFloat)

Sets the spacing between entries

Deprecated

func setTitleAlignment(NSTextAlignment)

Sets the alignment for all of the entry titles.

Deprecated

func setTextAlignment(NSTextAlignment)

Sets the alignment for all of the receiver’s editable text.

Deprecated

func setTextBaseWritingDirection(NSWritingDirection)

Sets the writing direction for the text content of every control embedded in the form.

Deprecated

func setTitleFont(NSFont)

Sets the font for all of the entry titles.

Deprecated

func setTextFont(NSFont)

Sets the font for all of the receiver’s editable text fields

Deprecated

