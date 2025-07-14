

- AppKit
- NSFontManager
-  localizedName(forFamily:face:) 

Instance Method

# localizedName(forFamily:face:)

Returns a localized string with the name of the specified font family and face, if one exists.

macOS

``` source
func localizedName(
    forFamily family: String,
    face faceKey: String?
) -> String
```

## Parameters 

`family`  

The font family, for example, `@"Times"`.

`faceKey`  

The font face, for example, `@"Roman"`.

## Return Value

A localized string with the name of the specified font family and face, or, if `face` is `nil`, the font family only.

## Discussion

The user’s locale is determined from the user’s `NSLanguages` default setting. The method also loads the localized strings for the font, if they aren’t already loaded.

## See Also

### Setting and Examining the Selected Font

func setSelectedFont(NSFont, isMultiple: Bool)

Records the specified font as the currently selected font and updates the Font panel.

var selectedFont: NSFont?

The currently selected font object.

var isMultiple: Bool

A Boolean value that indicates whether the currently selected font has multiple fonts.

func sendAction() -> Bool

A Boolean value that indicates whether a responder handled the font manager’s action message.

