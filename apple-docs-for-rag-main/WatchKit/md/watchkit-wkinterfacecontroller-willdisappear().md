

- WatchKit
- WKInterfaceController
-  willDisappear() 

Instance Method

# willDisappear()

Tells the interface controller that its view is now offscreen.

watchOS 2.0+

``` source
@MainActor
func willDisappear()
```

## Mentioned in 

Navigating Between Scenes

## Discussion

WatchKit calls this method shortly before removing your interface controller’s content from the screen. Use this method to stop animations or perform other interface-related tasks prior to deactivation.

The system calls this method on your WatchKit extension’s main thread. The `super` implementation of this method does nothing.

## See Also

### Responding to activation and appearance events

func willActivate()

Tells the interface controller that the system is about to activate its view.

func didDeactivate()

Tells the interface controller that its view is no longer active.

func didAppear()

Tells the interface controller that its view is now onscreen.

