

- UIKit
- UIPopoverController
-  present(from:in:permittedArrowDirections:animated:) Deprecated

Instance Method

# present(from:in:permittedArrowDirections:animated:)

Displays the popover and anchors it to the specified location in the view.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func present(
    from rect: CGRect,
    in view: UIView,
    permittedArrowDirections arrowDirections: UIPopoverArrowDirection,
    animated: Bool
)
```

## Parameters 

`rect`  

The rectangle in view at which to anchor the popover window.

`view`  

The view containing the anchor rectangle for the popover.

`arrowDirections`  

The arrow directions the popover is permitted to use. You can use this value to force the popover to be positioned on a specific side of the rectangle. However, it is generally better to specify any and let the popover decide the best placement. You must not specify unknown for this parameter.

`animated`  

Specify true to animate the presentation of the popover or false to display it immediately.

## See Also

### Presenting and dismissing the popover

func present(from: UIBarButtonItem, permittedArrowDirections: UIPopoverArrowDirection, animated: Bool)

Displays the popover and anchors it to the specified bar button item.

Deprecated

func dismiss(animated: Bool)

Dismisses the popover programmatically.

Deprecated

