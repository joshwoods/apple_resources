

- UIKit
- UIColorWell
-  selectedColor 

Instance Property

# selectedColor

The selected color in the color picker.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var selectedColor: UIColor? { get set }
```

## Discussion

When a person selects a new color in the color picker, the system generates the control event valueChanged.

This property is KVO-compliant.

## See Also

### Configuring color picker attributes

var title: String?

The title for the color picker.

var supportsAlpha: Bool

A Boolean value that determines whether the color picker supports alpha values.

