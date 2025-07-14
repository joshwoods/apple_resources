

- AppKit
- NSFont
-  userFont(ofSize:) 

Type Method

# userFont(ofSize:)

Returns the font used by default for documents and other text under the user’s control (that is, text whose font the user can normally change), in the specified size.

macOS

``` source
class func userFont(ofSize fontSize: CGFloat) -> NSFont?
```

## Parameters 

`fontSize`  

The size in points to which the font is scaled.

## Return Value

A font object of the specified size.

## Discussion

If `fontSize` is 0 or negative, returns the user font at the default size.

## See Also

### Related Documentation

init?(name: String, size: CGFloat)

Creates a font object for the specified font name and font size.

class func setUser(NSFont?)

Sets the font used by default for documents and other text under the user’s control to the specified font.

### Creating User Fonts

class func userFixedPitchFont(ofSize: CGFloat) -> NSFont?

Returns the font used by default for documents and other text under the user’s control (that is, text whose font the user can normally change), when that font should be fixed-pitch, in the specified size.

