

- UIKit
- UIPrintInteractionControllerDelegate
-  printInteractionControllerParentViewController(\_:) 

Instance Method

# printInteractionControllerParentViewController(\_:)

Returns a parent view controller for managing the printing-options view.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printInteractionControllerParentViewController(_ printInteractionController: UIPrintInteractionController) -> UIViewController?
```

## Parameters 

`printInteractionController`  

The shared instance of UIPrintInteractionController that is managing the print job.

## Return Value

The view controller that is to be the parent of the print-interaction controller managing the printing-options view. Return `nil` for the standard presentation behavior.

## Discussion

This method allows an application to present the print-options view from a view controller of their own choosing. The parent view controller returned must be a UIViewController object, such as a UINavigationController object or a generic view controller. A common strategy for embedding is to create a UINavigationController object as the content view controller (contentViewController property) of a UIPopoverController object and return that. UIKit can push the returned view controller onto the stack if its parent is a navigation controller or present it modally if it isn’t.

This method is invoked in any of the `present...` methods of the UIPrintInteractionController class (for example, present(animated:completionHandler:)).

