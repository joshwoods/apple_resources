

- AppKit
- NSForm
-  setFrameSize(\_:) Deprecated

Instance Method

# setFrameSize(\_:)

Sets the size of the receiver’s frame size to the specified value.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func setFrameSize(_ newSize: NSSize)
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`newSize`  

The new size of the form.

## Discussion

The width of `NSFormCell` objects always match the width of their encompassing `NSForm` object. The cell width is always changed to match the view regardless of the value returned by autosizesCells.

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

func setInterlineSpacing(CGFloat)

Sets the spacing between entries

Deprecated

func setTitleAlignment(NSTextAlignment)

Sets the alignment for all of the entry titles.

Deprecated

func setTitleBaseWritingDirection(NSWritingDirection)

Sets the writing direction for the title of every control embedded in the form.

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

