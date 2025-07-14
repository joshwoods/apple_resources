

- UIKit
- UIPopoverController
-  dismiss(animated:) Deprecated

Instance Method

# dismiss(animated:)

Dismisses the popover programmatically.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func dismiss(animated: Bool)
```

## Parameters 

`animated`  

Specify true to animate the dismissal of the popover or false to dismiss it immediately.

## Discussion

You can use this method to dismiss the popover programmatically in response to taps inside the popover window. Taps outside of the popover’s contents automatically dismiss the popover.

## See Also

### Presenting and dismissing the popover

func present(from: CGRect, in: UIView, permittedArrowDirections: UIPopoverArrowDirection, animated: Bool)

Displays the popover and anchors it to the specified location in the view.

Deprecated

func present(from: UIBarButtonItem, permittedArrowDirections: UIPopoverArrowDirection, animated: Bool)

Displays the popover and anchors it to the specified bar button item.

Deprecated

