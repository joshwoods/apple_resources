

- UIKit
- UIViewController
-  isMovingFromParent 

Instance Property

# isMovingFromParent

A Boolean value indicating whether the view controller is moving from a parent view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isMovingFromParent: Bool { get }
```

## See Also

### Responding to view-related events

func viewWillAppear(Bool)

Notifies the view controller that its view is about to be added to a view hierarchy.

func viewIsAppearing(Bool)

Notifies the view controller that the system is adding the view controller’s view to a view hierarchy.

func viewDidAppear(Bool)

Notifies the view controller that its view was added to a view hierarchy.

func viewWillDisappear(Bool)

Notifies the view controller that its view is about to be removed from a view hierarchy.

func viewDidDisappear(Bool)

Notifies the view controller that its view was removed from a view hierarchy.

var isBeingDismissed: Bool

A Boolean value indicating whether the view controller is in the process of being dismissed by one of its ancestors.

var isBeingPresented: Bool

A Boolean value indicating whether the view controller in the process of being presented by one of its ancestors.

var isMovingToParent: Bool

A Boolean value indicating whether the view controller is moving to a parent view controller.

