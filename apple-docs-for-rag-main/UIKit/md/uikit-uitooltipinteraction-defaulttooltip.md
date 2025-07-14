

- UIKit
- UIToolTipInteraction
-  defaultToolTip 

Instance Property

# defaultToolTip

The text that appears in a tooltip by default.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var defaultToolTip: String? { get set }
```

## Discussion

Set this property to the default text to display in the tooltip.

If you set the delegate property to an object that conforms to the UIToolTipInteractionDelegate protocol and implements the toolTipInteraction(_:configurationAt:) method, then the return value of the delegate method determines the text that appears in the tooltip.

## See Also

### Managing the interaction

var isEnabled: Bool

A Boolean value that indicates whether the tooltip interaction is in the enabled state.

