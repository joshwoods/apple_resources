

- UIKit
- UIPresentationController
-  init(presentedViewController:presenting:) 

Initializer

# init(presentedViewController:presenting:)

Initializes and returns a presentation controller for transitioning between the specified view controllers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    presentedViewController: UIViewController,
    presenting presentingViewController: UIViewController?
)
```

## Parameters 

`presentedViewController`  

The view controller being presented modally.

`presentingViewController`  

The view controller whose content represents the starting point of the transition.

## Return Value

An initialized presentation controller object or `nil` if the presentation controller could not be initialized.

## Discussion

This method is the designated initializer for the presentation controller. You must call it from any custom initialization methods you define for your presentation controller subclasses.

