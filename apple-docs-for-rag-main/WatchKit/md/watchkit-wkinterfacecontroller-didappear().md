

- WatchKit
- WKInterfaceController
-  didAppear() 

Instance Method

# didAppear()

Tells the interface controller that its view is now onscreen.

watchOS 2.0+

``` source
@MainActor
func didAppear()
```

## Mentioned in 

Navigating Between Scenes

Working with the watchOS app life cycle

## Discussion

WatchKit calls this method shortly after the interface controller’s contents appear onscreen. Use this method to configure animations or other interface-related tasks.

The system calls this method on your WatchKit extension’s main thread. The `super` implementation of this method does nothing.

## See Also

### Responding to activation and appearance events

func willActivate()

Tells the interface controller that the system is about to activate its view.

func didDeactivate()

Tells the interface controller that its view is no longer active.

func willDisappear()

Tells the interface controller that its view is now offscreen.

