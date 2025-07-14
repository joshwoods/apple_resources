

- AppKit
- NSWindow
-  setAnchorAttribute(\_:for:) 

Instance Method

# setAnchorAttribute(\_:for:)

Sets the part of the window that stays stationary during constraint-based layout.

macOS

``` source
@MainActor
func setAnchorAttribute(
    _ attr: NSLayoutConstraint.Attribute,
    for orientation: NSLayoutConstraint.Orientation
)
```

## Parameters 

`attr`  

The layout attribute. NSLayoutConstraint.Attribute specifies the possible values.

`orientation`  

The window drag orientation. NSLayoutConstraint.Orientation specifies the possible values.

## See Also

### Constraint-Based Layouts

func anchorAttribute(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Attribute

Returns the part of the window that stays stationary during constraint-based layout.

