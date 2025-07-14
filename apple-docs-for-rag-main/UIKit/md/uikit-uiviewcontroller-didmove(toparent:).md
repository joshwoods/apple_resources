

- UIKit
- UIViewController
-  didMove(toParent:) 

Instance Method

# didMove(toParent:)

Called after the view controller is added or removed from a container view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func didMove(toParent parent: UIViewController?)
```

## Parameters 

`parent`  

The parent view controller, or `nil` if there is no parent.

## Mentioned in 

Creating a custom container view controller

## Discussion

Your view controller can override this method when it wants to react to being added to a container.

If you are implementing your own container view controller, it must call the didMove(toParent:) method of the child view controller after the transition to the new controller is complete or, if there is no transition, immediately after calling the addChild(_:) method.

The removeFromParent() method automatically calls the didMove(toParent:) method of the child view controller after it removes the child.

## See Also

### Responding to containment events

func willMove(toParent: UIViewController?)

Called just before the view controller is added or removed from a container view controller.

