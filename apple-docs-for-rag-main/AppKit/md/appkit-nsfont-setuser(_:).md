

- AppKit
- NSFont
-  setUser(\_:) 

Type Method

# setUser(\_:)

Sets the font used by default for documents and other text under the user’s control to the specified font.

macOS

``` source
class func setUser(_ font: NSFont?)
```

## Discussion

Specifying `aFont` as `nil` causes the default to be removed from the application domain.

## See Also

### Related Documentation

class func userFont(ofSize: CGFloat) -> NSFont?

Returns the font used by default for documents and other text under the user’s control (that is, text whose font the user can normally change), in the specified size.

### Setting User Fonts

class func setUserFixedPitch(NSFont?)

Sets the font used by default for documents and other text under the user’s control, when that font should be fixed-pitch, to the specified font.

