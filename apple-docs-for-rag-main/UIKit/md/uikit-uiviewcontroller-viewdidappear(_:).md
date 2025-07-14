

- UIKit
- UIViewController
-  viewDidAppear(\_:) 

Instance Method

# viewDidAppear(\_:)

Notifies the view controller that its view was added to a view hierarchy.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func viewDidAppear(_ animated: Bool)
```

## Parameters 

`animated`  

If true, the view was added to the window using an animation.

## Mentioned in 

Positioning content relative to the safe area

Displaying and managing views with a view controller

## Discussion

You can override this method to perform additional tasks associated with presenting the view. If you override this method, you must call `super` at some point in your implementation.

Note

If a view controller is presented by a view controller inside of a popover, this method is not invoked on the presenting view controller after the presented controller is dismissed.

## See Also

### Responding to view-related events

func viewWillAppear(Bool)

Notifies the view controller that its view is about to be added to a view hierarchy.

func viewIsAppearing(Bool)

Notifies the view controller that the system is adding the view controller’s view to a view hierarchy.

func viewWillDisappear(Bool)

Notifies the view controller that its view is about to be removed from a view hierarchy.

func viewDidDisappear(Bool)

Notifies the view controller that its view was removed from a view hierarchy.

var isBeingDismissed: Bool

A Boolean value indicating whether the view controller is in the process of being dismissed by one of its ancestors.

var isBeingPresented: Bool

A Boolean value indicating whether the view controller in the process of being presented by one of its ancestors.

var isMovingFromParent: Bool

A Boolean value indicating whether the view controller is moving from a parent view controller.

var isMovingToParent: Bool

A Boolean value indicating whether the view controller is moving to a parent view controller.

