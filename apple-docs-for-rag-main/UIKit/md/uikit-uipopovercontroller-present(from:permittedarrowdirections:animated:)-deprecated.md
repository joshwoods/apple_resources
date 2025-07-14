

- UIKit
- UIPopoverController
-  present(from:permittedArrowDirections:animated:) Deprecated

Instance Method

# present(from:permittedArrowDirections:animated:)

Displays the popover and anchors it to the specified bar button item.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func present(
    from item: UIBarButtonItem,
    permittedArrowDirections arrowDirections: UIPopoverArrowDirection,
    animated: Bool
)
```

## Parameters 

`item`  

The bar button item on which to anchor the popover.

`arrowDirections`  

The arrow directions the popover is permitted to use. You can use this value to force the popover to be positioned on a specific side of the bar button item. However, it is generally better to specify any and let the popover decide the best placement. You must not specify unknown for this parameter.

`animated`  

Specify true to animate the presentation of the popover or false to display it immediately.

## Discussion

When presenting the popover, this method adds the toolbar that owns the button to the popover’s list of passthrough views. Thus, taps in the toolbar result in the action methods of the corresponding toolbar items being called. If you want the popover to be dismissed when a different toolbar item is tapped, you must implement that behavior in your action handler methods.

## See Also

### Presenting and dismissing the popover

func present(from: CGRect, in: UIView, permittedArrowDirections: UIPopoverArrowDirection, animated: Bool)

Displays the popover and anchors it to the specified location in the view.

Deprecated

func dismiss(animated: Bool)

Dismisses the popover programmatically.

Deprecated

