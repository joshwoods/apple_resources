

- UIKit
- UIPrintInteractionController
-  present(from:in:animated:completionHandler:) 

Instance Method

# present(from:in:animated:completionHandler:)

Presents the iPad printing user interface in a popover view, optionally animating it from any area in a view.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func present(
    from rect: CGRect,
    in view: UIView,
    animated: Bool,
    completionHandler completion: UIPrintInteractionController.CompletionHandler? = nil
) -> Bool
```

## Parameters 

`rect`  

A rectangle that defines the area from which the printing popover view is animated.

`view`  

The view providing the coordinate system for `rect`.

`animated`  

true to animate the printing popover view from `item`, false to display it immediately.

`completion`  

A block of type UIPrintInteractionController.CompletionHandler that you implement to handle the conclusion of the print job (for instance, to reset state) and to handle any errors encountered in printing.

## Discussion

It is valid to call this method for applications on iPad devices. Calling this method on an iPhone or iPod touch with `animated` set to true causes the printing options view to animate upward from the bottom of the screen.

If you call this method when the printing options are already displayed, `UIPrintInteractionController` hides the printing-options popover view. You must call the method again to display the options.

## See Also

### Presenting the printing user interface

func present(animated: Bool, completionHandler: UIPrintInteractionController.CompletionHandler?) -> Bool

Presents the iPhone printing user interface in a sheet, optionally animating it to slide up from the bottom of the screen.

func present(from: UIBarButtonItem, animated: Bool, completionHandler: UIPrintInteractionController.CompletionHandler?) -> Bool

Presents the iPad printing user interface in a popover view, optionally animating it from a bar-button item.

func dismiss(animated: Bool)

Dismisses the printing-options sheet or popover.

