

- UIKit
- UIControl
-  toolTip 

Instance Property

# toolTip

The default text to display in the control’s tooltip.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var toolTip: String? { get set }
```

## Discussion

Set this property to the text that should appear in the tooltip. If you want your app to determine the tooltip text at a later time — for instance, to determine the text based on the current state of your app — set the delegate property of toolTipInteraction after setting toolTip with the default text. For example, the following code listing sets the tooltip’s default text and delegate for a shopping cart button:

```
let button = UIButton(configuration: configuration, primaryAction: action)
button.toolTip = "Click to add the item to your cart. Your cart is empty."
button.toolTipInteraction?.delegate = self
```

If the delegate implements the method toolTipInteraction(_:configurationAt:), the tooltip ignores the default text set in the toolTip property. For more information, see toolTipInteraction.

## See Also

### Showing tooltips

var toolTipInteraction: UIToolTipInteraction?

The tooltip interaction associated with the control.

