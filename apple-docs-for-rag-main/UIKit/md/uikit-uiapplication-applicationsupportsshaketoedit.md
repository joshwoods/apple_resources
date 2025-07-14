

- UIKit
- UIApplication
-  applicationSupportsShakeToEdit 

Instance Property

# applicationSupportsShakeToEdit

A Boolean value that determines whether shaking the device displays the undo-redo user interface.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var applicationSupportsShakeToEdit: Bool { get set }
```

## Discussion

The default value is true. Set the property to false if you don’t want your app to display the Undo and Redo buttons when users shake the device.

## See Also

### Controlling and handling events

func sendEvent(UIEvent)

Dispatches an event to the appropriate responder objects in the app.

func sendAction(Selector, to: Any?, from: Any?, for: UIEvent?) -> Bool

Sends an action message identified by the selector to a specified target.

