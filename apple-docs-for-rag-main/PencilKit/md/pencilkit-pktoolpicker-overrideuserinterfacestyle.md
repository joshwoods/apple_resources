

- PencilKit
- PKToolPicker
-  overrideUserInterfaceStyle 

Instance Property

# overrideUserInterfaceStyle

The specific user interface style to apply to the tool picker.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var overrideUserInterfaceStyle: UIUserInterfaceStyle { get set }
```

## Discussion

If you set this property, consider if you need to set colorUserInterfaceStyle to a select a different user interface style. The default user interface style is UIUserInterfaceStyle.unspecified.

## See Also

### Customizing picker behavior

var isRulerActive: Bool

A Boolean value that indicates whether the ruler is visible on the canvas.

var colorUserInterfaceStyle: UIUserInterfaceStyle

The user interface style for the tool picker.

var showsDrawingPolicyControls: Bool

A Boolean value that indicates whether the default drawing policy UI is visible.

var stateAutosaveName: String?

The name used to automatically save the tool picker’s state in the defaults system.

