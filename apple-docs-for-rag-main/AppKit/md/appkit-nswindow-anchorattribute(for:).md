

- AppKit
- NSWindow
-  anchorAttribute(for:) 

Instance Method

# anchorAttribute(for:)

Returns the part of the window that stays stationary during constraint-based layout.

macOS

``` source
@MainActor
func anchorAttribute(for orientation: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Attribute
```

## Parameters 

`orientation`  

The attribute for orientation. NSLayoutConstraint.Orientationspecifies the possible values.

## Return Value

Returns the layout attribute.

## See Also

### Constraint-Based Layouts

func setAnchorAttribute(NSLayoutConstraint.Attribute, for: NSLayoutConstraint.Orientation)

Sets the part of the window that stays stationary during constraint-based layout.

