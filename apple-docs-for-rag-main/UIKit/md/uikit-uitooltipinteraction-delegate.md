

- UIKit
- UIToolTipInteraction
-  delegate 

Instance Property

# delegate

An object that provides text that a tooltip displays instead of the default text.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIToolTipInteractionDelegate)? { get set }
```

## Discussion

To provide tooltip text based on the current state or unique logic of your app, set the delegate property to an object that conforms to the UIToolTipInteractionDelegate protocol and implements the toolTipInteraction(_:configurationAt:) method. The method returns a UIToolTipConfiguration object containing the text to display in the tooltip. For example, the following code listing instructs the tooltip to show the name of the view’s background color instead of the defaultToolTip text. If the color name is unavailable, the method returns `nil`, which disables the display of the tooltip.

```
func toolTipInteraction(_ interaction: UIToolTipInteraction, configurationAt point: CGPoint) -> UIToolTipConfiguration? {
    let configuration: UIToolTipConfiguration?
    if let accessibilityName = backgroundColor?.accessibilityName {
        configuration = UIToolTipConfiguration(toolTip: "The color is \(accessibilityName).")
    } else {
        configuration = nil
    }

    return configuration
}
```

## See Also

### Providing tooltip configurations

protocol UIToolTipInteractionDelegate

An interface that provides tooltip settings to an interaction.

