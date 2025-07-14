

- UIKit
- UIColorWell
-  supportsAlpha 

Instance Property

# supportsAlpha

A Boolean value that determines whether the color picker supports alpha values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var supportsAlpha: Bool { get set }
```

## Discussion

If this property is false, people can only pick fully opaque colors from the color picker.

## See Also

### Configuring color picker attributes

var title: String?

The title for the color picker.

var selectedColor: UIColor?

The selected color in the color picker.

