

- AppKit
- NSForm
-  setInterlineSpacing(\_:) Deprecated

Instance Method

# setInterlineSpacing(\_:)

Sets the spacing between entries

macOS 10.0–10.10Deprecated

``` source
@MainActor
func setInterlineSpacing(_ spacing: CGFloat)
```

Deprecated

Use NSTextField directly instead, and consider NSStackView for layout assistance

## Parameters 

`spacing`  

The spacing between entries, measured in points in the user coordinate space.

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

