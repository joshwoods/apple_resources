

- AppKit
- NSForm
-  setBordered(\_:) Deprecated

Instance Method

# setBordered(\_:)

Sets whether the receiver’s entries should display a border around their editable text fields.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func setBordered(_ flag: Bool)
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`flag`  

true to display a border around all entries; otherwise, false to show no border around all entries.

## Discussion

The border is drawn as a thin line around the editable text field. An entry can have a border or a bezel, but not both.

## See Also

### Related Documentation

var isBordered: Bool

A Boolean value indicating whether the cell draws itself outlined with a plain border.

### Changing the Appearance of All the Entries

func setBezeled(Bool)

Sets whether the receiver’s entries should display a bezel around their editable text.

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

