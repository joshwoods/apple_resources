

- AppKit
- NSForm
-  setBezeled(\_:) Deprecated

Instance Method

# setBezeled(\_:)

Sets whether the receiver’s entries should display a bezel around their editable text.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func setBezeled(_ flag: Bool)
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`flag`  

true to display a bezel around all entries; otherwise, false to show no bezel around all entries.

## See Also

### Related Documentation

var isBezeled: Bool

A Boolean value indicating whether the cell has a bezeled border.

### Changing the Appearance of All the Entries

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

