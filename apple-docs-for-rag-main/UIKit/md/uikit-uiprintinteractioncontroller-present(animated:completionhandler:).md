

- UIKit
- UIPrintInteractionController
-  present(animated:completionHandler:) 

Instance Method

# present(animated:completionHandler:)

Presents the iPhone printing user interface in a sheet, optionally animating it to slide up from the bottom of the screen.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func present(
    animated: Bool,
    completionHandler completion: UIPrintInteractionController.CompletionHandler? = nil
) -> Bool
```

## Parameters 

`animated`  

true to animate the display of the sheet, false to display the sheet immediately.

`completion`  

A block of type UIPrintInteractionController.CompletionHandler that you implement to handle the conclusion of the print job (for instance, to reset state) and to handle any errors encountered in printing.

## Discussion

It is valid to call this method for applications on iPhone and iPod touch devices. Calling this method on an iPad with `animated` set to true causes the printing options view to animate from the window frame.

If you call this method when the printing options are already displayed, `UIPrintInteractionController` hides the printing-options sheet. You must call the method again to display the options.

## See Also

### Presenting the printing user interface

func present(from: UIBarButtonItem, animated: Bool, completionHandler: UIPrintInteractionController.CompletionHandler?) -> Bool

Presents the iPad printing user interface in a popover view, optionally animating it from a bar-button item.

func present(from: CGRect, in: UIView, animated: Bool, completionHandler: UIPrintInteractionController.CompletionHandler?) -> Bool

Presents the iPad printing user interface in a popover view, optionally animating it from any area in a view.

func dismiss(animated: Bool)

Dismisses the printing-options sheet or popover.

