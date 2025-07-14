

- WatchKit
- WKInterfaceController
-  willActivate() 

Instance Method

# willActivate()

Tells the interface controller that the system is about to activate its view.

watchOS 2.0+

``` source
@MainActor
func willActivate()
```

## Mentioned in 

Working with the watchOS app life cycle

Navigating Between Scenes

## Discussion

The system calls this method when it is getting ready to display your interface controller. Use this method to perform last minute tasks required to ensure your content is up to date. Do not use this method to perform the initial setup of your interface. Your interface should be mostly initialized and ready to use by the time this method is called.

The calling of this method is not a guarantee that your interface controller is onscreen or about to appear onscreen. The system may call this method early to give you time to update your content. Use the didAppear() method to determine when your interface appears onscreen.

The system calls this method on your WatchKit extension’s main thread. The `super` implementation of this method does nothing.

## See Also

### Responding to activation and appearance events

func didDeactivate()

Tells the interface controller that its view is no longer active.

func didAppear()

Tells the interface controller that its view is now onscreen.

func willDisappear()

Tells the interface controller that its view is now offscreen.

