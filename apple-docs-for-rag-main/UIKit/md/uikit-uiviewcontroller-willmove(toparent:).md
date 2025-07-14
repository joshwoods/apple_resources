

- UIKit
- UIViewController
-  willMove(toParent:) 

Instance Method

# willMove(toParent:)

Called just before the view controller is added or removed from a container view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func willMove(toParent parent: UIViewController?)
```

## Parameters 

`parent`  

The parent view controller, or `nil` if there is no parent.

## Mentioned in 

Creating a custom container view controller

## Discussion

Your view controller can override this method when it needs to know that it has been added to a container.

If you are implementing your own container view controller, it must call the willMove(toParent:) method of the child view controller before calling the removeFromParent() method, passing in a parent value of `nil`.

When your custom container calls the addChild(_:) method, it automatically calls the willMove(toParent:) method of the view controller to be added as a child before adding it.

## See Also

### Responding to containment events

func didMove(toParent: UIViewController?)

Called after the view controller is added or removed from a container view controller.

