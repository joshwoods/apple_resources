

- UIKit
- UIControl
-  toolTipInteraction 

Instance Property

# toolTipInteraction

The tooltip interaction associated with the control.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var toolTipInteraction: UIToolTipInteraction? { get }
```

## Discussion

When you set the toolTip property, the control creates a UIToolTipInteraction object and assigns it to the toolTipInteraction property.

If you want to change the text of the tooltip based the current state of your app or application logic, assign a UIToolTipInteractionDelegate object to toolTipInteraction‘s delegate property. For example, the following code listing sets the tooltip’s default text and delegate for a shopping cart button:

```
lazy var shoppingCartButtonWithTooltip: UIButton = {
    var configuration = UIButton.Configuration.filled()
    configuration.title = "Add to Cart"
    configuration.image = UIImage(systemName: "cart", variant: .circle)
    configuration.imagePlacement = NSDirectionalRectEdge.leading
    configuration.imagePadding = 4

    let action = UIAction { [unowned self] _ in self.cartItemCount += 1 }

    let button = UIButton(configuration: configuration, primaryAction: action)
    button.toolTip = "Click to add the item to your cart. Your cart is empty."
    button.toolTipInteraction?.delegate = self

    return button
}()
```

Then the delegate returns a tooltip configuration containing text that states the number of items in the shopping cart by implementing the toolTipInteraction(_:configurationAt:) method:

```
func toolTipInteraction(_ interaction: UIToolTipInteraction, configurationAt point: CGPoint) -> UIToolTipConfiguration? {

    let text: String
    switch cartItemCount {
    case 0:
        text = "Click to add the item to your cart. Your cart is empty."
    case 1:
        text = "Click to add the item to your cart. Your cart contains \(cartItemCount) item."
    default:
        text = "Click to add the item to your cart. Your cart contains \(cartItemCount) items."
    }

    return UIToolTipConfiguration(toolTip: text)
}
```

## See Also

### Showing tooltips

var toolTip: String?

The default text to display in the control’s tooltip.

