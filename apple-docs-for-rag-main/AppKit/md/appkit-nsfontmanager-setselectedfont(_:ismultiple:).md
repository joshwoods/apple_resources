

- AppKit
- NSFontManager
-  setSelectedFont(\_:isMultiple:) 

Instance Method

# setSelectedFont(\_:isMultiple:)

Records the specified font as the currently selected font and updates the Font panel.

macOS

``` source
func setSelectedFont(
    _ fontObj: NSFont,
    isMultiple flag: Bool
)
```

## Parameters 

`fontObj`  

The font to set as selected.

`flag`  

If true, the Font panel indicates that more than one font is contained in the selection; if false, it does not.

## Discussion

An object that manipulates fonts should invoke this method whenever it becomes first responder and whenever its selection changes. It shouldn’t invoke this method in the process of handling a changeFont: message, as this causes the font manager to lose the information necessary to effect the change. After all fonts have been converted, the font manager itself records the new selected font.

## See Also

### Setting and Examining the Selected Font

var selectedFont: NSFont?

The currently selected font object.

var isMultiple: Bool

A Boolean value that indicates whether the currently selected font has multiple fonts.

func sendAction() -> Bool

A Boolean value that indicates whether a responder handled the font manager’s action message.

func localizedName(forFamily: String, face: String?) -> String

Returns a localized string with the name of the specified font family and face, if one exists.

