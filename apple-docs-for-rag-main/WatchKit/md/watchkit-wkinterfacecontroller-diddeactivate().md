

- WatchKit
- WKInterfaceController
-  didDeactivate() 

Instance Method

# didDeactivate()

Tells the interface controller that its view is no longer active.

watchOS 2.0+

``` source
@MainActor
func didDeactivate()
```

## Mentioned in 

Working with the watchOS app life cycle

## Discussion

The system calls this method as part of the cleanup process for the interface controller. Use this method to invalidate timers or save any app-related state information that has not already been saved. Any tasks you perform using this method should finish quickly. An inactive interface controller may be reactivated later or it may be deallocated.

Do not use this method to modify your interface. WatchKit ignores attempts to set values of interface objects while your interface is inactive, including during the execution of this method. Modifications can be made only during initialization of your interface controller and between calls to willActivate() and this method.

The system calls this method on your WatchKit extension’s main thread. The `super` implementation of this method does nothing.

In iOS Simulator, WatchKit calls this method for the current interface controller when you lock the simulator by selecting Hardware \> Lock. When you subsequently unlock the simulator, WatchKit calls that interface controller’s willActivate() method again. You can use this capability to debug your activation and deactivation code.

## See Also

### Responding to activation and appearance events

func willActivate()

Tells the interface controller that the system is about to activate its view.

func didAppear()

Tells the interface controller that its view is now onscreen.

func willDisappear()

Tells the interface controller that its view is now offscreen.

