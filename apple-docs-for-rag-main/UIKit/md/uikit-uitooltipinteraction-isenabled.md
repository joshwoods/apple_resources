

- UIKit
- UIToolTipInteraction
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the tooltip interaction is in the enabled state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

A view or control can only display a tooltip from an enabled interaction. Set the value of the isEnabled property to true to enable the interaction or false to disable it. The default value is true.

## See Also

### Managing the interaction

var defaultToolTip: String?

The text that appears in a tooltip by default.

